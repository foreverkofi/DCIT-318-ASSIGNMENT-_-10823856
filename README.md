using System;

// Define IMovable interface
public interface IMovable
{
    void Move(); // Method signature for movement
}

// Car class implementing IMovable interface
public class Car : IMovable
{
    public void Move()
    {
        Console.WriteLine("Car is moving");
    }
}

// Bicycle class implementing IMovable interface
public class Bicycle : IMovable
{
    public void Move()
    {
        Console.WriteLine("Bicycle is moving");
    }
}

class Program
{
    static void Main(string[] args)
    {
        // Create an instance of Car
        Car car = new Car();
        car.Move();  // Output: Car is moving

        // Create an instance of Bicycle
        Bicycle bicycle = new Bicycle();
        bicycle.Move();  // Output: Bicycle is moving
    }
}
