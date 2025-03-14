 # Create a Book
# COMMAND
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)

# Expected Output:
<Book: 1984 by George Orwell (1949)>

# Retrieve the Book
# COMMAND
book = Book.objects.get(title="1984")

# Expected Output:
Title: 1984, Author: George Orwell, Year: 1949

# Update the Book Title
# COMMAND
book.title = "Nineteen Eighty-Four"
book.save()

# Expected Output:
Updated Title: Nineteen Eighty-Four

# Delete the Book
# COMMAND
book.delete()

# Expected Output:
<QuerySet []>