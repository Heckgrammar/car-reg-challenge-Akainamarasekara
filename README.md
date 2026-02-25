<img width="1082" height="163" alt="image" src="https://github.com/user-attachments/assets/340632b8-42fb-445e-9757-eb4a8d6f920d" />
<img width="341" height="60" alt="image" src="https://github.com/user-attachments/assets/5cdf7eef-4297-4655-b9e4-ebdd09ff0537" />
namespace Car_Reg_Challenge
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int charge = 0;
            Console.Write("Enter your car registration: ");
            string carReg = Console.ReadLine();
            while (carReg.Length > 8)
            {
                string displayMessge = " is not valid";
                Console.Write(displayMessge);
                carReg = Console.ReadLine();
            }
            Console.Write("Enter your stay in hours: ");
            int hours = Convert.ToInt32(Console.ReadLine());
            if (hours < 2)
            {
                charge = 0;
            }
            else
            {
                charge = hours * 2;
            }
            Console.WriteLine(charge);
