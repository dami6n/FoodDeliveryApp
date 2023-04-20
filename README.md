# FoodDeliveryApp
Food delivery app made in Kotlin.
# Programación de Dispositivos Móviles

## Alumnos:

- García Méndez Gerardo Damián
- Hernández Sánchez Oscar José

## Notas e Instrucciones para correr la aplicación:

Para correr nuestra aplicacición se deben comentar ciertas lineas de código en la clase MainActivity.ktt descritas 
a continuación:

1. La aplicación cuenta con dos ventanas (Activity) la cuales son fragment_dashboard.xml y activity_forma_de_pago.xml
2. Para visualizar activity_main basta con comentar la liena 20 del archivo MainActivity.kt
3. Para visualizar activity_forma_de_pago se debe comentar de la linea 23 a 37 del archivo MainActivity.kt
4. Se utilizó la versión 8.0.0 (oreo) de Android Para correrla 
5.Utilizamos la versión Android Studio Flamingo |2022.2.1 para realizar esta tarea

## Muestra de las lineas que se deben comentar
Dentro del archivo MainActivity.kt.
Para ver activity_main el código a comentar es:

 setContentView(R.layout.activity_forma_de_pago);

Para ver activity_forma_de_pago el código a comentar es:

     binding = ActivityMainBinding.inflate(layoutInflater)
        setContentView(binding.root)

        val navView: BottomNavigationView = binding.navView

        val navController = findNavController(R.id.nav_host_fragment_activity_main)
        // Passing each menu ID as a set of Ids because each
        // menu should be considered as top level destinations.
        val appBarConfiguration = AppBarConfiguration(
            setOf(
                R.id.navigation_home, R.id.navigation_dashboard, R.id.navigation_notifications
            )
        )
        setupActionBarWithNavController(navController, appBarConfiguration)
        navView.setupWithNavController(navController)

        
