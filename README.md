# Camas por Roster (paradas)

`index.html` reemplaza el trabajo manual de la pestaña DATA y la tabla dinámica TD del
`Roster_General_Proyecto.xlsx`. Se abre en https://marycielolobo-spec.github.io/roster-camas/ o con doble clic al archivo. Funciona sin internet porque la librería
de Excel (SheetJS) va incrustada en el archivo, y el Excel no se sube a ningún lado.

Uso:
1. Cargar el roster actual (hoja ROSTER, el mismo que alimenta el dashboard).
2. (Opcional) Cargar el roster anterior para ver solo lo que cambió.
3. Revisar las camas por día contra la meta (318 por defecto) y descargar el Excel con las hojas RESUMEN, DATA y CAMBIOS.

Reglas, sacadas de la DATA manual:
- Ocupan cama: D, N, DF, NF, IN, S, DMP, QP (D8, N9, S1… cuentan como su código base). Se editan en la página.
- La bajada (BN/BD) no ocupa cama: la cama se usa hasta el día anterior a bajar.
- «Alojamiento en Chilloroya = SI»: trabaja normal pero no cuenta cama en Constancia.
