
MainActivity3

//Main method
import javax.swing.JOptionPane;
public class MainActivity3 {
	public static void main(String[] args) {
	
		JOptionPane.showMessageDialog(null,"NOTEBOOK");
		System.out.println("__________________NOTEBOOK______________________");
		
		Notebook1 notebook = new Notebook1();
		notebook.nameBrand();
		notebook.sayColor();
		notebook.qLeaves();
				
		Notebook note = new Notebook();
		note.length();
		note.width();		
	}
}






//Superclass
interface Shape{
	void length();
}
public interface Size extends Shape{
	void width();

}

class Notebook implements Size{
	public void length() {
		System.out.println("This notebook has 8.5 inches length");
	}
	public void width() {
		System.out.println("and 6 inches width");
	}
}






//Subclass
public class Notebook1 extends Notebook{
	String brand;
	String color;
	int leaves;
	
	public Notebook1() {
		this.brand = "Cattleya";
		this.color = "Black";
		this.leaves = 120;
	}
	
	public void nameBrand() {
		System.out.println("Notebook brand: " + brand);
	}
	public void sayColor() {
		System.out.println("Color: " + color);
	}
	public void qLeaves() {
		System.out.println("with " + leaves + " leaves");
	}
}




//Jemay Arriesgado
//Christina Pepito
//Gerica Canete
//Roselyn Arenas
