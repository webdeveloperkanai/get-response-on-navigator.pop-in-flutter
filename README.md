# get response on navigator.pop() function in flutter 

suppose this is a button 
<code> 
  ElevatedButton(
      onPressed: () {
         final result = await Navigator.push(
                        context,
                        MaterialPageRoute(builder: (context) => const SelectionScreen()),
                      );
      },
      child: const Text('Pick an option, any option!'),
    );
</code> 

in this result variable we will get reponse poped by SelectionScreen(); 

We have to pass value in pop method like 

<code>
  Navigator.pop(context, 'This is returning value on pop()');
 </code> 
 
 We can access this string in that result variable and we can perform the recomended tasks. 
