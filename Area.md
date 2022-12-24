
using System;
namespace program
{
    class MathArea
    {
        private double RADIUS; //شعاع

        public double Radius
        {
            Get { Return Radius; }
            Set { Radius = value; }
        }

        public double EnvironmentCircle()
        {
            return 2 * 3.14 * Radius;
        }
        public double AreaCircle()
        {
            return   Radius*Radius*3.14;
        }


    }
    class result
    {
        public static void Main()
        {
            Console.WriteLine("plese enter your path:circle,triangle,Square,Trapezius");
            string UserChoose = Console.ReadLine();
            
            if (UserChoose == "circle")
            {
                MathArea circle = new MathArea();
                Console.WriteLine("please enter radius");
                circle.Radius = Convert.ToDouble(Console.ReadLine());
                double ResEnvironment = circle.EnvironmentCircle();
                double ResArea = circle.AreaCircle();

                Console.WriteLine("Environment:"+ResEnvironment);
                Console.WriteLine("Area:"+circle.AreaCircle);
         }

        }
    }
}
