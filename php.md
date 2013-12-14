Function() :

String->
        Repeat : str_repeat(string,2)
        Make substring : substr(string,2,5)
        Find position: strpos(string ,"example")
        Find character : strchr(string,"a")

Number->
        Absolute value : abs(0-300);
        Exponential : pow(2,8);
        Square root : sqrt(100);
        Modulo: fmod(20,7);
        Random(any) : rand();
        Random(min,max): rand(1,10);

  **PHP provides four constructs you can use to load an external script: include, include_once,
require, and require_once.
The PHP manual recommends that developers use include_once and require_once because
these constructs first check whether the file has already been loaded before either will load a given
script. This saves resources and can increase the performance of your applications.**


Super global array :
        • $GLOBALS: Variables available in the global scope
        • $_SERVER: Information about the server
        • $_GET: Data passed using the HTTP GET method
        • $_POST: Data passed using the HTTP POST method
        • $_REQUEST: Data passed via an HTTP request
        • $_FILES: Data passed by an HTML file input
        • $_SESSION: Current session data specific to the user
        • $_COOKIE: Data stored on the user’s browser as a cookie

Declare array : $months = array("january","February");
                or : $months = ["january","February"];  //php 5.4

Condition check : if( == )   and if ( === )  and if(!==)
                          else()

                         switch statement
                         while loop
           foreach loop : ex : $arr = ["Hiren","12 June"];
            					foreach($arr as $name){
            					    echo $name;
            					}
            			OR :     $arr = [ "Hiren" => "Personality" , "12 June" => "12 August"]
            			           foreach($arr as $taiNa => $name)
            			           { 
            			               echo $name ;   //output  Personality12 June
            			           }

Print :  echo ""
           printf()  [Formated output just like C]
           print()    [Just print string ]
           print_r() [Print array's item]
           sprintf() [ useful for storing an output in variable ]


 Define funtion : function(paramiter){
                         ..........
                         return ...;
                           }

conneting to database : $conn = new PDO('databaseDriver:hostsname;databasename;',databaseUsername,dataBasePassword);

** For substition use double quote not single quote " "
**Inside echo use echo "{$variable_name}";

Dynamic variable : $var;
                            $$var  //this is dynamic variable

** static varibale and global varibale example : static $var ; golbal $var ;

Include/requre/requre_once : include "about.php" ;


$_GET['Variable']   //Use only for fetch data like item list etc. Not for updating database
**Check is variable is not empty using isset(var)
**For security use htmlspecialchars($_GET['var'])