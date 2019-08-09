# Create_a_ruby_gem

1.-Crearemos primero una carpeta que contendra nuestros archivos 

+ __NOTA:__ El nombre de la carpeta puede ser el que sea, en este caso le asignaremos el nombre de *primera_gema*

2.-Dentro de nuestra carpeta crearemos un archivo *.gemspec*
+ El nombre de nuestra gema(archivo .gemspec) que usaremos como ejemplo será el siguiente: __ejemplo.gemspec__.

3.-Rellenaremos nuestro documento __ejemplo.gemspec__ de la siguiente manera:

# Archivo primera_gema/ejemplo.gemspec

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
  
  
  s.files = Dir["{lib}/**/*.rb", "bin/*", "LICENSE", "*.md"]
  
end


+ Puedes encontrar en el siguiente link la manera de rellenar la información para nuestra gema http://guides.rubygems.org/specification-reference.


  
