**Htmler**

*Ronaldo Barbachano*

*Feb 2012*

*AGPL*
	
A very simple php5.3 class that takes advantage of overloaded magic method '__callStatic'.
	
Htmler processes method names to dynamically call private functions	that generate html.
	
***Usage***



*Example make a 'div' container with 'hello world'*
	
	echo htmler::div__('hello world');
	
*Example make a 'div' container with 'hello world', with class name 'worlds'*
	
	echo htmler::div__worlds('hello world');
	
*Example make a 'div' container with 'hello world', with class name 'worlds', id 'my_world'*
	
	echo htmler::div__worlds__my_world('hello world');

*Dynamic method naming example..*

	$method_call = 'div__words';
		
	echo htmler::$method_call('hello world');
	
*Html 'element' example*

	// Also supports 'link' elements (mostly for the head)..
	// others to follow shortly

	echo htmler::link__stylesheet('style.css');
	
