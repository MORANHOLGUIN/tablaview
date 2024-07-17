<img width="731" alt="image" src="https://github.com/user-attachments/assets/03e56072-a097-449e-a676-07d04758021f">
<img width="769" alt="image" src="https://github.com/user-attachments/assets/f2608a04-12cf-4333-802b-3f6dbd72c445">
<img width="764" alt="image" src="https://github.com/user-attachments/assets/e1a52a57-9a28-461e-ba21-9688639d6359">
<img width="719" alt="image" src="https://github.com/user-attachments/assets/37598791-1e7b-4b57-8e88-b463f1fe44d9">

Paquetes y Clases
JavaFX:

Application: Clase principal de JavaFX.
ComboBox, TableView, TableColumn, VBox, Scene, Stage: Componentes de JavaFX para crear la interfaz gráfica.
JDBC:

Connection, DriverManager, ResultSet, PreparedStatement: Clases de JDBC para conectar y ejecutar consultas en la base de datos.
Colecciones de JavaFX:

FXCollections, ObservableList: Utilizados para gestionar y actualizar datos en la interfaz gráfica de JavaFX.
Componentes del Código

Clase Main

ComboBox:
Un componente desplegable para seleccionar el año de la temporada.

TableView:
Una tabla para mostrar los resultados de los constructores con columnas para el nombre del constructor, victorias, puntos totales y posición.

VBox:
Un contenedor vertical que agrupa el ComboBox y la TableView.

Métodos Importantes

start(Stage primaryStage):
Método principal de JavaFX para inicializar y mostrar la interfaz gráfica.

getSeasons():
Método para obtener los años de las temporadas desde el repositorio.

getConstructorResultsByYear(int year):
Método para obtener los resultados de los constructores para un año específico desde el repositorio.

Modelo

ConstructorResult:
Una clase modelo para representar los resultados de los constructores con atributos para el nombre, victorias, puntos totales y posición.

Repositorios

ConstructorResultRepository:
Clase para interactuar con la base de datos y recuperar los resultados de los constructores.
Método getResultByYear(int year) para ejecutar la consulta SQL y devolver los resultados.

Bases de Datos y SQL

Conexión a PostgreSQL:

jdbcUrl, user, password: Detalles de la conexión a la base de datos.

Consulta SQL:
Una consulta SQL para obtener los resultados de los constructores por año, utilizando JOIN para combinar tablas y GROUP BY para agrupar los resultados.
Uso de RANK() para ordenar los constructores por puntos en cada temporada.
