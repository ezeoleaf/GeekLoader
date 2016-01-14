# GeekLoader
GeekLoader is a loader made with Javascript and CSS so you can replace the boring loaders with John Conway's Game of Life or with Langton's ant

## How to use it
Just create an object of GeekLoader

```javascript
loader = new GeekLoader();
```

### Options
You can configure the loader with this options
- type --This is the type of loader
- sizeH --Quantity of rows
- sizeV --Quantity of columns
- time --The time between each move(milliseconds)
- destiny --The id of the div that contains the loader
- border --If every cell has border or not

### How to configure it
```javascript
loader.type = 'life';
loader.setSize(rows,columns) or loader.sizeH=10;
loader.time = 500;
loader.destiny = 'divLoader';
loader.border = true;
```

### Actions
```javascript
loader.setSize(row,columns); //Set the rows and columns
loader.generate(); //It's executed with the constructor, but you can call it anytime. It generates the board
loader.start(); //Starts the movement of the loader
loader.stop(); //Stop the loader and hides it
```