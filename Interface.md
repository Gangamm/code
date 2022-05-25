using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp3
{
    interface Interface1
    {
        //method without body
        void calculateArea(int l, int b);
    }
    class Rectangle : Interface1
    {
        public void calculateArea(int l,int b)//it must provide the body for the interface data member
        {
            int area = l * b;
            Console.WriteLine( "Area of Rectangle:"+area);

        }
    }
    class Program1
    {
        static void Main(string[] args)
        {
            Rectangle r = new Rectangle();
            r.calculateArea(100, 200);
        }
    }
}
