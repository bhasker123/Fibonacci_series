
using System;


namespace SamplePrograms
{
    class Fibonacci
    {
        public static void Main()
        {
            // Prompt the user to enter their target number
            Console.WriteLine("How many numbers do you want in the fibonacci series");


            // Read the user input from console and convert to integer
            int Target = int.Parse(Console.ReadLine());


            // Create integer variables to hold previous and next numbers
            int PreviousNumber = -1, NextNumber = 1;


            // This for loop controls the number of fibonacci series elements
            for (int i = 0; i < Target; i++)
            {
                // Logic to compute fibonacci series numbers
                int Sum = PreviousNumber + NextNumber;
                PreviousNumber = NextNumber;
                NextNumber = Sum;
                Console.Write(NextNumber + "  ");
            }


            Console.ReadLine();
        }
    }
}