 from bookshelf.models import Book

# Creating a Book instance
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
print(book)  # Expected output: <Book: 1984 by George Orwell (1949)>
