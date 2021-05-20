package newpackage;

public class classanotherproject {
	public void getname()
	{
		System.out.println("Im from another package.");
	}
}

package pack;
import newpackage.classanotherproject;

public class Newclass {
	public String name="Sai";
	public void details()
	{
		System.out.println(name);
	}
}

class Jala {
	public static void main(String[] args) {
		Newclass a = new Newclass();
		a.details(); // same package diff class
		classanotherproject c = new classanotherproject();
		c.getname(); // diff package diff class
	}
}
