# Ex.No:4(C)  COMPOSITION IN JAVA

## QUESTION:
Implement a system where a Library contains multiple Book objects. Each Book is created inside the Library. Books can't exist independently (Composition).
## AIM:
To implement Composition in Java by creating a Library class that contains and owns multiple Book objects

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3. Create an empty Library object.
4. Read the number of books n.
5. Repeat for each book: Read the book title AND author.
6. Library creates a new Book object and stores it.
7. After all books are added, display all stored books with their details.
8. End


## PROGRAM:
 ```
/*
Program to implement a Composition Concepts in Java
Developed by: LOGESHWARI R
RegisterNumber: 212223060137
*/
```

## SOURCE CODE:
```
import java.util.*;

public class CompositionExample {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Library library = new Library();

        int n = sc.nextInt();
        sc.nextLine(); // Consume the newline

        for (int i = 0; i < n; i++) {
            String title = sc.nextLine();
            String author = sc.nextLine();
            library.addBook(title, author);
        }

        library.showBooks();
        sc.close();
    }
}


class Book {
    private String title;
    private String author;

    public Book(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getDetails() {
        return title + " by " + author;
    }
}


class Library {
    private List<Book> books;

    public Library() {
        this.books = new ArrayList<>();
    }

    public void addBook(String title, String author) {
       
        Book newBook = new Book(title, author);
        this.books.add(newBook);
    }

    public void showBooks() {
        System.out.println("Books in Library:");
        if (books.isEmpty()) {
            System.out.println("- No books found.");
        } else {
            for (Book book : books) {
                System.out.println("- " + book.getDetails());
            }
        }
    }
}
```


## OUTPUT:

<img width="946" height="542" alt="image" src="https://github.com/user-attachments/assets/aef15263-f139-481a-8264-8ad4687ed341" />


## RESULT:

The program successfully creates Book objects within the Library class and displays all added books, demonstrating composition

