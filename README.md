# stringProblem

Define a Java class to solve this problem:<br>
Given a String and a Character, remove all instances of the Character in the String

Solve this two ways:<br>
1. Iterate through the String, one character at a time<br>
2. Find a method in the String class that can solve this in one line<br>

Write methods for each solution.

Afterwards, write a TestNG or JUnit class for each solution which tests these methods.<br>
Include both positive and negative cases for validations.
  
  
  Soultion:

      
       public String withoutX(String str)
       {
          int len = str.length();
	  if(len > = 2)
	  {
	  char ch = str.charAt(0);
	  StringBuilder stbuild = new StringBuilder(len);
	  if(ch!='x')
	     Stbuild.append(ch);
	     Stbuild.append(str.substring(1,len-1));
	      ch = str.charAt(len-1);
	  if(ch! = 'x')
	      stbuild.append(ch);
	    return stbuild.toString();
	    }
	    else if(len == 1 && str.charAt(0)=='x')
	        return"";
		else
		return str;
       }
  Method 2:
   
        public String withoutX(String str)
	{
	  str = str.replace("x","");
	  return str;

	}   


