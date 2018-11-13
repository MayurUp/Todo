# Todo
Simple while loop example.

All outputs into console.

Whats your input? 
Fill: "list" or "New" or 'delete' or you can quit type "quit"
then type accordingly:
var todo = ['hello1'];

var input = prompt('Whats your input?');

while (input !== 'quit'){
	if (input === 'list') {
		console.log('*********************');
		todo.forEach(function(todo, i){
			console.log(i + ': ' + todo);
		});
		console.log('*********************');
	}
	else 
		if (input === 'new') {
			var newTode = prompt('What new todo');
			todo.push(newTode);		
		}
	else 
		if (input === 'delete') {
			var index = prompt('What to delete from todo type index no.');
			todo.splice(index,1);
			console.log('Deleted todo');
			// todo.pop(newTode);		
		}
		input = prompt('What would you like to do?');
	}
console.log('OK your quit the App');
