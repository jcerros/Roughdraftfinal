public class Bi_Pedmain {
  public static void main(String args[]) {
		
		Monkey Object = new Monkey(7, 75, 50, 20);
		Human Object2 = new Human(21, 170,15, 5);
		Robot Object3 = new Robot(9, 55, 45, 15);

		Object.name();
		Object.talk();
		System.out.println("monkey age :" + Object.getAge() + " yrs"
				+ "\nMonkey wieght:" + Object.getWeight() + " lbs"
				+ "\nmonkey Speed:" + Object.getSpeed() + " mph"
				+ "\nMonkey acceleration:" + Object.getAcceleration());
	
		Object2.name();
		Object2.talk();
		System.out.println("human age :" + Object2.getAge() + " yrs"
				+ "\nHuman wieght:" + Object2.getWeight() + " lbs"
				+ "\nHuman Speed:" + Object2.getSpeed() + " mph"
				+ "\nHuman acceleration:" + Object2.getAcceleration());

		Object3.name();
		Object3.talk();
		System.out.println("robot age :" + Object3.getAge() + " yrs"
				+ "\nrobot wieght:" + Object3.getWeight() + " lbs"
				+ "\nrobot Speed:" + Object3.getSpeed() + " mph"
				+ "\nrobot acceleration:" + Object3.getAcceleration());

	
	}

}


public abstract class Animal {
  

	private int age;
	private int weight;
	private int speed;
	private int acceleration;


	public Animal(int age, int weight, int speed,
			int acceleration) {
		super();
		this.age = age;
		this.weight = weight;
		this.speed = speed;
		this.acceleration = acceleration;

	}

	public int getAge() {
		return age;
	}

	public void setAge(int age) {
		this.age = age;
	}

	public int getWeight() {
		return weight;
	}

	public void setWeight(int weight) {
		this.weight = weight;
	}

	public int getSpeed() {
		return speed;
	}

	public void setSpeed(int speed) {
		this.speed = speed;
	}

	public void setAcceleration(int acceleration) {
		this.acceleration = acceleration;
	}

	public int getAcceleration() {
		return acceleration;
	}

	
	public void name() {
		System.out.println("Uknown/no name!");
	}

	
	public void talk() {
		System.out.println("cannot talk!");
	}

	
	public int walk(int speed) {
		int s = 0;
		s = speed;
		return (0 + (int) (Math.random() * s));
	}
}


public class Monkey extends Animal {

  

	public Monkey(int age, int weight, int speed,
			int acceleration) {
		super(age, weight,speed, acceleration);

	}

	public void name() {
		System.out.println("aaah ooh ooooh(my name is George)!");
	}

	public void talk() {
		System.out.println("Oooh ooh aah aaah!");

	}

	public int walk(int speed) {
		int k;
		k = speed;
		return (0 + (int) (Math.random() * k));
		
	}

	

	
}
public class Human extends Animal {

  public Human(int age, int weight, int speed,
			int acceleration) {
		super(age, weight, speed, acceleration);

	}

	public void name() {
		System.out.println("\n\n\nMy name is Mesut Ozil!!");
	}

	public void talk() {
		System.out.println("Hello!");

	}

	public int walk(int speed) {
		int f;
		f = speed;
		return 0 + (int) (Math.random() * f);
		
	}

	
	
}


public class Robot extends Animal {
  

	public Robot(int age, int weight, int speed,
			int acceleration) {
		super(age, weight, speed, acceleration);

	}

	public void name() {
		System.out.println("\n\n\nMy name is E-102 GAM-MA.");
	}

	public void talk() {
		System.out.println("HEL-LO.");

	}

	public int walk(int speed) {
		int t;
	t = speed;
		return (0 + (int) (Math.random() * t));
		

	}

	
}

