# C# out 

<pre><code>
using System; 
using System.Collections.Generic; 
using System.Text; 

class OutExample
{
  static void Method(out int i)
  {
    i = 44;
  }
  static void Method(ref int i)
  {
    // is possible overload
  }
  
  
  static void Main()
  {
    int value;
    // value is null
    Method(out value);
    System.Console.WriteLine(value); 
    // value is 44
    
  }  
}
</code></pre>

