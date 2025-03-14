from bookshelf.models import Book

# Retrieving and updating the book
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
print(f"Updated Title: {book.title}")
# Expected output: Updated Title: Nineteen Eighty-Four