# code
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp3
{
  abstract class Array
    {
        public abstract void Add(int a,int b);//when the method is  Abstract no body for that method
        
    }
    class sub:Array
    {
        public override void Add(int a,int b)//when the base class is abstract give a body for that
        {
            int sum = a + b;
            Console.WriteLine("Sum of two number: "+sum); 
        }
       
    }
    class Abstract
    {
        static void Main(string[] args)
        {
            sub s = new sub();
            s.Add(4,8);
        }
     
       
    }
}
