# Chess System Java

This chess system is implemented in Java using object-oriented programming concepts and exception treatment. It has two layers: the chess layer and the board layer.

## System Design

The system design is shown in the following UML diagram:

![image](https://github.com/marialuizaleitao/chess-system-java/assets/88951059/fc4e6b98-50cd-45a3-ae53-c2ec7fe8c636)

## OOP Concepts Used in Chess System Project

This chess system project uses a variety of OOP concepts, including:

1. _Encapsulation_: This concept is used to hide the internal state of objects and who can access the attributes and methods of that object. For example, the Board and Piece classes encapsulate their attributes so that they can only be accessed through public getter and setter methods.
2. _Constructors_: These are special methods that are used to initialize objects when they are created. In particular, the Position, Board, and Piece classes all have constructors that allow you to initialize their attributes when you create a new instance of the class.
3. _Overriding_:  This concept allows you to override methods of a parent class in a subclass. Using this concept, you can override the default toString() method of the Object class to return a custom string representation of your object. For instance, the King, Bishop, Knight, Pawn, Queen, and Rook classes all override the move() method of the ChessPiece class to implement their own specific movement rules. The Position class overrides the toString() method to return a string representation of the position in the format (row, column).
4. _Associations_: This concept describes the relationship between two objects. To illustrate, the Board and Piece classes have an association relationship, which means that a Board object can have many Piece objects, and a Piece object can only belong to one Board object.
5. _Enumerations_: This concept is used to define a set of named constants. In the project, the ChessSystem class uses an enumeration to represent the color of a chess piece (black or white).
6. _Inheritance_: This concept allows you to create new classes that are based on existing classes. As seen, the King, Bishop, Knight, Pawn, Queen, and Rook classes all inherit from the ChessPiece class.
7. _Downcasting_: This concept allows you to cast a reference variable to a subclass of its current type. For example, the Board class uses downcasting to cast a Piece reference variable to a specific type of chess piece, such as a King or Queen.
8. _Static members_: These are members of a class that can be accessed without first creating an instance of the class. For example, the ChessSystem class has a static method that can be used to create a new chess board.
9. _Layers pattern_: This design pattern is used to organize code into different layers, such as a presentation layer, a business logic layer, and a data access layer. The chess system project uses a layered architecture to separate the chess logic from the user interface and the underlying data storage.
10. _Polymorphism_: This concept allows objects of different types to respond to the same method in different ways. In the project, the Position, Board, and Piece classes all override the toString() method to return a custom string representation of their respective objects.
11. _Exceptions_: This concept is used to handle errors during program execution. The chess system project uses exceptions to handle errors such as invalid chess moves and checkmate.
12. _Abstract method/class_: This concept is used to define classes and methods that cannot be instantiated directly. For example, the ChessPiece class is an abstract class that defines the basic behavior of all chess pieces.
13. _Overloading_: This concept allows you to define multiple methods with the same name but different parameters. For example, the ChessSystem class has two overloaded methods called move(), one that takes two Position objects as parameters and the other that takes a String object as a parameter.

### Data Structures

The chess system project uses a matrix to represent the chessboard. The Board class uses a two-dimensional array to store the pieces on the chessboard. This data structure is efficient for representing a chessboard because it allows you to quickly access any position on the board.

The chess system project also uses a list to store the players in a chess game. This data structure is efficient for storing the players because it allows you to easily add, remove, and access players in the list.
