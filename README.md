# Camas por Roster (paradas)

`index.html` reemplaza el trabajo manual de la pestaña DATA y la tabla dinámica TD del
`Roster_General_Proyecto.xlsx`. Se abre en https://marycielolobo-spec.github.io/roster-camas/ o con doble clic al archivo. Funciona sin internet porque la librería
de Excel (SheetJS) va incrustada en el archivo, y el Excel no se sube a ningún lado.

Uso:
1. Cargar el roster actual (hoja ROSTER, el mismo que alimenta el dashboard).
2. (Opcional) Cargar el roster anterior para ver solo lo que cambió.
3. «Personas por rango de días»: quiénes estarán en sitio entre dos fechas (con cama o en Chilloroya), descargable en Excel.
4. Revisar las camas por día contra la meta (318 por defecto) y descargar el Excel con las hojas RESUMEN, DATA y CAMBIOS.

Reglas, sacadas de la DATA manual:
- Ocupan cama: D, N, DF, NF, IN, S, DMP, QP (D8, N9, S1… cuentan como su código base). Se editan en la página.
- La bajada (BN/BD) no ocupa cama: la cama se usa hasta el día anterior a bajar.
- Chilloroya no cuenta cama (trabajan normal, duermen en la comunidad):
  - Lista permanente de todo el mes: la pestaña «Alojamiento en Chilloroya» del Excel, o DNI pegados en la página
    (se guardan en ese navegador). Manda sobre la columna del roster.
  - Además, quien tenga SI en la columna «Alojamiento en Chilloroya» del roster.
- El número al final del código es el día de la guardia (S1, D1…D19, BN1, L1…): se cuenta como su código base.
- Acepta el Roster General (hoja ROSTER) y la descarga del sistema (hoja Roster, sin columna de Chilloroya ni de
  contrato). «Agrupar por» elige la columna del resumen: CONTRATO GENERAL si existe; si no, PROYECTO.
