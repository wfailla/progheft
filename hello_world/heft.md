# Hello World!

## Wozu "Hello World!"?

Fast alle Bücher, Tutorials, Vorkurshefte und sonstige Programmierbeispiele beginnen mit einem einfachen Programm, das nichts tut als "Hello World!" auf der Konsole auszugeben.

Im Grund behandelt man mit dem "Hello World!"-Programm zwei Fragen: 
* Was und an welchen Stellen kann ich im Quelltext ändern, um ein tolleres Programm zu erhalten?
* Wie komme ich von der Quelltext-Datei zum laufenden Programm?

In den meisten Programmiersprachen gibt es eine Art "Rahmen" der die eigentliche Programmlogik umgibt.
In Java sieht das Hello-World-Programm wie folgt aus: 
<pre> <code>public class Hello {
	public static void main(String args[]) {
		System.out.println("Hello World!");	// gibt 'Hello World' aus.
	}
}</pre> </code>

Die erste Zeile enthält unter anderem den Namen des Programms nämlich "Hello". Die Datei mit dem Quelltext muss demzufolge "Hello.java" heißen.
"public static void main(String args[]) {" ist der Anfang der Main-Funktion des Programmes. Hier stehen die Befehle, die nach Programmstart als erstes abgearbeitet werden.
System.out.println("Hello World!"); – Das ist der Befehl der ausgeführt wird. "System.out.println" ist der Befehl der Text ausgibt, "Hello World!" der Text den wir ausgeben wollen. Die beiden Schließenden Klammern sind das Ende der Main-Funktion und das Ende des Programmes. 
Wenn wir also ein anderes Programm schreiben wollen, müssen wir lediglich den Befehl "System.out.println ..." durch andere Befehle ersetzen.

Um das Programm auszuführen, müssen wir zuerst den Quelltext des Programms in Bytecode umwandeln lassen und dann die Java-Virtual-Maschine aufrufen, die den Bytecode aufsführt. 
Für das Übersetzen des Quelltextes in Bytecode ist der Java-Compiler zuständig
Unter UNIX ruft man den Java-Compiler aus dem Terminal mit "javac Hello.java" auf. Der Compiler hat nun, sofern das Programm keine Fehler enthält eine Datei mit dem Namen "Hello.class" erzeugt (oder eine ältere Version überschrieben) – diese Datei enthält den Bytecode.
Die JVM kann man mit dem Befehl "java" aufrufen. "java Hello" führt den Bytecode in Hello.class aus.