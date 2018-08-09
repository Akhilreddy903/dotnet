# dotnet class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("enter the amount");
            int amount = int.Parse(Console.ReadLine());
            if (amount%5==0)
            {
                if (amount >= 500)
                {
                    int n500 = amount / 500;
                    Console.WriteLine("the no of five hundreads are:" + n500);
                    amount = amount % 500;
                }
                if (amount >= 100)
                {
                    int n100 = amount / 100;
                    Console.WriteLine("the no of hundreads are:" + n100);
                    amount = amount % 100;
                }
                if (amount >= 50)
                {
                    int n50 = amount / 50;
                    Console.WriteLine("the no of fifties are:" + n50);
                    amount = amount % 50;
                }
                if (amount >= 10)
                {
                    int n10 = amount / 10;
                    Console.WriteLine("the no of tens are:" + n10);
                    amount = amount % 10;
                }
                if (amount >= 5)
                {
                    int n5 = amount / 5;
                    Console.WriteLine("the no of fives are:" + n5);
                    amount = amount % 5;
                }
            }
            else
            {
                Console.WriteLine("the amount you entered is unable to dispense");
            }
            Console.Read();
        }
      
