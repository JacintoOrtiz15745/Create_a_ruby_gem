# Create_a_ruby_gem

1.-Crearemos primero una carpeta que contendra nuestros archivos 

+ __NOTA:__ El nombre de la carpeta puede ser el que sea, en este caso le asignaremos el nombre de *primera_gema*

2.-Dentro de nuestra carpeta *primera_gema* crearemos un archivo *.gemspec*
+ El nombre de nuestra gema(archivo .gemspec) que usaremos como ejemplo será el siguiente: __ejemplo.gemspec__.

3.-Rellenaremos nuestro archivo __ejemplo.gemspec__ de la siguiente manera:
   
    Gem::Specification.new do |s|
      s.name = "ejemplo"
      s.version = '0.0.1'
      s.date = '2019-08-09'
      s.authors = ["Jacinto Ortiz"]
      s.email = ["andresjacinto_araujo@ucol.com"]
      s.summary = "My very first"
      s.description = "Simple Hello World"
      s.homepage = "https://github.com/dbarrientos/gemadesafio"
      #s.files = ["lib/mygem3.rb"]
      # or
      s.files = Dir["{lib}/**/*.rb", "bin/*", "LICENSE", "*.md"]
    end


+ Puedes encontrar en el siguiente link la manera correcta de rellenar la información que se muestra arriba para nuestra gema http://guides.rubygems.org/specification-reference.
  
+  En la siguiente linea se incluiran todos los archivos que tengamos dentro de la carpeta __lib__ (en este caso sería __ejemplo_gemspec__)
   
         s.files = Dir["{lib}/**/*.rb", "bin/*", "LICENSE", "*.md"]
      
4.-Dentro de nuestra carpeta crearemos otra carpeta que se llamará: __lib__.

5.-Dentro de nuestra carpeta __lib__ crearemos un archivo(archivo ruby ".rb") en este caso se llamará __ejemplo.gemspec__

6.-A continuación crearemos el código para nuestra librería; dentro de nuestro archivo __ejemplo.gemspec__ ingresaremos nuestro código, en este caso el código utilizado será simple, pero solo es por fines demostrativos.

    class Gemadesafio
       
      def self.hola
        
        return "Hola mundo!!!"
        
      end
    end
   
7.-Ahora el siguiente paso es construir nuestra gema. Para esto abriremos nuestra terminal y nos situaremos en la carpeta que anteriormente habiamos creado (__primera_gema__). Una vez hecho esto escribiremos en nuestra terminal el siguiente comando 
     
      gem build 
  
