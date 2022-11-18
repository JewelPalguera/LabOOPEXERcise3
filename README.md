# LabOOPEXERcise3

BikeClass 
public class Bike{
		private String colour;//attribute
		private final Wheel wheel; //component or part

		//constructor
		public Bike(String colour){
			this.colour = colour;
			wheel = new Wheel ();
		}
		
		//accessor
		public String getcolour () {
			return colour;
		}

		//mutator
		public void setcolour(String colour){
			this.colour = colour;
		}
		
}

Wheel Class
import java.reflect.*;public class Wheel
{
	private String size; // Attribute
	
	//Constructor
	public Wheel(){
		size="Big Wheel in front";
	}
	
	//Accessor
	public String getWheel(){
		return size;
	}
	
	//mutator
	public void setSize(String size){
		this.size=size;
	}
	
	public String rollwheel() {
		return"The Bike's wheel is rolling.";
	}
	
	public String stopwheel(){
		return"The Bike's wheel is stop.";
	}
	
}

Main Program
public static void main(String[] args) {
		Bike colour = new Bike("Gray");
		Bike size = new Bike("The Bike's wheel is rolling.");
		
		System.out.println("" + colour.getcolour() + " " +  size.getcolour());
	}
}
