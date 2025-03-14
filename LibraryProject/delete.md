from bookshelf.models import Book

# Retrieving and deleting the book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

# Confirming deletion
books = Book.objects.all()
print(books)  # Expected output: <QuerySet []>