#Simple Markdown and other notes


####Setting up a new git connection
- git clone http://github.com/littlefieldja/"repo name"
	-	ex: git clone http://github.com/littlefieldja/school
	
####how to add files to github
######Work
 - must be in path user/e60891/git/school
 - git add .
 - git commit -m "message here"
 - git push
######Hoem
 - must be in path /Users/jameslittlefield/school
 - git pull . 
 - commits and pulls through vs code.

####Other commands 
- git status
	- shows status of modified and stacked docs.
	
	
####Simple things to remember 
- text formatting 
	- this is *italic* text.
	- this is **bold** text. 
	- this is both **_bold and italic_**.
	
- this is a order list 
	1. item 1 
	2. item 2	
	3. item 3
	
- how to format a list 
  1. item 1
   1. nested item 1a
   2. nested item 1b
  2. item 2
   1. nested item 2a
   2. nested item 2b
   
   
- this is a task list 
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item

:sob:
:milky_way:



####This is some code
```c++	
	int main (){
	double int1; 
	double int2; 
	std::cout << "Please enter a number";
	std::cin >> int1;
	std::cout << "Please enter another number";
	std::cin >> int2;
	
	std::cout >> "You entered " + int1 + " as the first number and " + int2 + " has the second number";
```
	
```ruby
	require 'redcarpet'
	markdown = Redcarpet.new("Hello World!")
	puts markdown.to_html
```

####Here are some mods made on my mac! 
Have made a change can you see it? 
 
 
