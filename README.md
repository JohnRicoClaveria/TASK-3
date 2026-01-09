using System;

class Task3
{
    static void Main()
    {
        // Declare and initialize the array
        int[] numbers = { 3, 7, 12, 19, 21, 25, 30 };

        // Ask the user for input
        Console.Write("Enter a number to search for: ");
        int target = Convert.ToInt32(Console.ReadLine());

        bool found = false;

        // Use a for loop to search the array
        for (int i = 0; i < numbers.Length; i++)
        {
            if (numbers[i] == target)
            {
                Console.WriteLine($"Number found at position {i}!");
                found = true;
                break; // Stop searching once found
            }
        }

        // If not found after loop
        if (!found)
        {
            Console.WriteLine("Number not found in the list.");
        }

        Console.ReadLine(); // Keeps the console window open
    }
}
