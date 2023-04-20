# FoodDeliveryApp
Food delivery app made in Kotlin.
# Programación de Dispositivos Móviles

## Alumnos:

- García Méndez Gerardo Damián
- Hernández Sánchez Oscar José

## Notas e Instrucciones para correr la aplicación:

Para correr nuestra aplicacición se deben comentar ciertas lineas de código en la clase MainActivity.ktt descritas 
a continuación:

1. La aplicación cuenta con dos ventanas (Activity) la cuales son MainActivity y FormaDePago
2. Para visualizar MainActivity basta con comentar la liena 20 del archivo MainActivity.kt
3. Para visualizar FormaDePago se debe comentar de la linea 23 a 37 del archivo MainActivity.kt

## Muestra de las lineas que se deben comentar
Dentro del archivo MainActivity.kt.
Para ver MainActivity el código a comentar es:

 setContentView(R.layout.activity_forma_de_pago);

Para ver FormaDePago el código a comentar es:

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

        