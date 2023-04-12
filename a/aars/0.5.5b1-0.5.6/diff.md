# Comparing `tmp/aars-0.5.5b1.tar.gz` & `tmp/aars-0.5.6.tar.gz`

## Comparing `aars-0.5.5b1.tar` & `aars-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 aars-0.5.5b1/mkdocs.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.5b1/py.typed
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aars-0.5.5b1/requirements.txt
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.5b1/.github/workflows/publish.yml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/Exceptions.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/index.md -> ../README.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/utils.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/core/AARS.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/core/Index.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.5b1/docs/core/Record.md
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 aars-0.5.5b1/src/aars/__init__.py
--rw-r--r--   0        0        0    33016 2020-02-02 00:00:00.000000 aars-0.5.5b1/src/aars/core.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aars-0.5.5b1/src/aars/exceptions.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 aars-0.5.5b1/src/aars/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.5b1/tests/__init__.py
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 aars-0.5.5b1/tests/aars.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 aars-0.5.5b1/tests/fetch_all.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.5b1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.5b1/LICENSE
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 aars-0.5.5b1/README.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aars-0.5.5b1/pyproject.toml
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 aars-0.5.5b1/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 aars-0.5.6/docs-requirements.txt
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aars-0.5.6/mkdocs.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/py.typed
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 aars-0.5.6/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/mkdocs-gh-pages.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 aars-0.5.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aars-0.5.6/docs/FastAPI_Cookbook.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/Exceptions.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/utils.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/AARS.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/Index.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aars-0.5.6/docs/Code_Reference/core/Record.md
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/__init__.py
+-rw-r--r--   0        0        0    37114 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/core.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/exceptions.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 aars-0.5.6/src/aars/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aars-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 aars-0.5.6/tests/aars.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aars-0.5.6/tests/fetch_all.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 aars-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 aars-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 aars-0.5.6/README.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aars-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 aars-0.5.6/PKG-INFO
```

### Comparing `aars-0.5.5b1/.github/workflows/publish.yml` & `aars-0.5.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aars-0.5.5b1/src/aars/exceptions.py` & `aars-0.5.6/src/aars/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,104 @@
-class AlephError(Exception):
-    """Base class for exceptions in this module."""
-    pass
-
-
-class AlephPermissionError(AlephError):
-    """Exception raised when a user is not authorized to perform an action on an item."""
-
-    def __init__(self,
-                 user_address: str,
-                 item_hash: str,
-                 item_owner: str,
-                 message="User {0} is not authorized to modify {1} by user {2}"):
-        self.user_address = user_address
-        self.item_hash = item_hash
-        self.item_owner = item_owner
-        self.message = message.format(self.user_address, self.item_hash, self.item_owner)
-        super().__init__(self.message)
-
-
-class AlreadyUsedError(AlephError):
-    """Exception raised when a PageableResponse has already been used."""
-
-    def __init__(
-        self,
-        message="PageableResponse has already been iterated over. It is recommended to "
-        "to store the result of all() or page() or to create a new query.",
-    ):
-        self.message = message
-        super().__init__(self.message)
-
-
-class AlreadyForgottenError(AlephError):
-    """
-    Exception raised when a user tries to forget an item that has already been forgotten.
-    """
-    def __init__(
-        self,
-        content,
-        message="Object '{0}' has already been forgotten. It is recommended to delete the "
-        "called object locally.",
-    ):
-        self.item_hash = content.id_hash
-        self.message = f"{message.format(self.item_hash)}"
-        super().__init__(self.message)
-
-
-class PostTypeIsNoClassError(AlephError):
-    """Exception raised when a received post_type is not resolvable to any python class in current runtime."""
-
-    def __init__(
-        self,
-        content,
-        message="Received post_type '{0}' from channel '{1}' does not currently exist as a "
-        "class.",
-    ):
-        self.post_type = content["type"]
-        self.content = content["content"]
-        self.channel = content["channel"]
-        self.message = f"""{message.format(self.post_type, self.channel)}\n
-        Response of {self.post_type} provides the following fields:\n
-        {[key for key in self.content.keys()]}"""
-        super().__init__(self.message)
-
-
-class InvalidMessageTypeError(AlephError):
-    """Exception raised when program received a different message type than expected."""
-
-    def __init__(
-        self,
-        received,
-        expected,
-        message="Expected message type '{0}' but actually received '{1}'",
-    ):
-        self.received = received
-        self.expected = expected
-        self.message = f"{message.format(self.expected, self.received)}"
-        super().__init__(self.message)
-
-
-class NotStoredError(AlephError):
-    """Exception raised when a requested object is not stored on Aleph and has no `item_hash`."""
-
-    def __init__(
-        self,
-        record,
-        message="Record '{0}'\nis not stored on Aleph. It is required to store the "
-        "record with .save() before calling this method.",
-    ):
-        self.type = record.content
-        self.message = f"{message.format(self.type)}"
-        super().__init__(self.message)
+"""
+Types of exceptions that can be raised when using the AARS library.
+All exceptions are subclasses of [AlephError][aars.exceptions.AlephError].
+"""
+
+
+class AlephError(Exception):
+    """Base class for exceptions in this module."""
+
+    pass
+
+
+class AlephPermissionError(AlephError):
+    """Exception raised when a user is not authorized to perform an action on an item."""
+
+    def __init__(
+        self,
+        user_address: str,
+        item_hash: str,
+        item_owner: str,
+        message="User {0} is not authorized to modify {1} by user {2}",
+    ):
+        self.user_address = user_address
+        self.item_hash = item_hash
+        self.item_owner = item_owner
+        self.message = message.format(
+            self.user_address, self.item_hash, self.item_owner
+        )
+        super().__init__(self.message)
+
+
+class AlreadyUsedError(AlephError):
+    """Exception raised when a PageableResponse has already been used."""
+
+    def __init__(
+        self,
+        message="PageableResponse has already been iterated over. It is recommended to "
+        "to store the result of all() or page() or to create a new query.",
+    ):
+        self.message = message
+        super().__init__(self.message)
+
+
+class AlreadyForgottenError(AlephError):
+    """
+    Exception raised when a user tries to forget an item that has already been forgotten.
+    """
+
+    def __init__(
+        self,
+        content,
+        message="Object '{0}' has already been forgotten. It is recommended to delete the "
+        "called object locally.",
+    ):
+        self.item_hash = content.id_hash
+        self.message = f"{message.format(self.item_hash)}"
+        super().__init__(self.message)
+
+
+class PostTypeIsNoClassError(AlephError):
+    """Exception raised when a received post_type is not resolvable to any python class in current runtime."""
+
+    def __init__(
+        self,
+        content,
+        message="Received post_type '{0}' from channel '{1}' does not currently exist as a "
+        "class.",
+    ):
+        self.post_type = content["type"]
+        self.content = content["content"]
+        self.channel = content["channel"]
+        self.message = f"""{message.format(self.post_type, self.channel)}\n
+        Response of {self.post_type} provides the following fields:\n
+        {[key for key in self.content.keys()]}"""
+        super().__init__(self.message)
+
+
+class InvalidMessageTypeError(AlephError):
+    """Exception raised when program received a different message type than expected."""
+
+    def __init__(
+        self,
+        received,
+        expected,
+        message="Expected message type '{0}' but actually received '{1}'",
+    ):
+        self.received = received
+        self.expected = expected
+        self.message = f"{message.format(self.expected, self.received)}"
+        super().__init__(self.message)
+
+
+class NotStoredError(AlephError):
+    """Exception raised when a requested object is not stored on Aleph and has no `item_hash`."""
+
+    def __init__(
+        self,
+        record,
+        message="Record '{0}'\nis not stored on Aleph. It is required to store the "
+        "record with .save() before calling this method.",
+    ):
+        self.type = record.content
+        self.message = f"{message.format(self.type)}"
+        super().__init__(self.message)
```

### Comparing `aars-0.5.5b1/tests/aars.py` & `aars-0.5.6/tests/aars.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,204 +1,191 @@
-import asyncio
-from typing import List, Optional
-
-from aleph.sdk import AuthenticatedAlephClient
-from aleph.sdk.conf import settings
-from aleph.sdk.chains.ethereum import get_fallback_account
-
-from src.aars import Record, Index, AARS
-from src.aars.exceptions import AlreadyForgottenError
-import pytest
-
-AARS(session=AuthenticatedAlephClient(get_fallback_account(), settings.API_HOST))
-
-
-@pytest.fixture(scope="session")
-def event_loop():
-    yield AARS.session.http_session.loop
-    asyncio.run(AARS.session.http_session.close())
-
-
-@pytest.fixture(scope="session", autouse=True)
-def create_indices(request):
-    Index(Book, 'title')
-    Index(Book, ['title', 'author'])
-    Index(Library, on='name')
-
-
-class Book(Record):
-    title: str
-    author: str
-    year: Optional[int]
-
-
-class Library(Record):
-    name: str
-    books: List[Book]
-
-
-def test_invalid_index_created():
-    try:
-        index = None
-        with pytest.raises(ValueError):
-            index = Index(Book, 'some_nonexistent_field')
-    finally:
-        if index:
-            Record.remove_index(index)
-
-
-def test_duplicate_index_creation():
-    with pytest.raises(ValueError):
-        Index(Book, 'title')
-
-
-@pytest.mark.asyncio
-async def test_store_and_index():
-    new_book = await Book(title='Atlas Shrugged', author='Ayn Rand').save()
-    assert new_book.title == 'Atlas Shrugged'
-    assert new_book.author == 'Ayn Rand'
-    await asyncio.sleep(1)
-    fetched_book = await Book.where_eq(title='Atlas Shrugged').first()
-    print(fetched_book)
-    print(new_book)
-    assert new_book == fetched_book
-
-
-@pytest.mark.asyncio
-async def test_multi_index():
-    new_book = await Book(title='Lila', author='Robert M. Pirsig', year=1991).save()
-    # wait a few secs
-    await asyncio.sleep(1)
-    should_be_none = await Book.where_eq(title='Lila', author='Yo Momma').all()
-    assert len(should_be_none) == 0
-    fetched_book = await Book.where_eq(title='Lila', author='Robert M. Pirsig').first()
-    assert new_book == fetched_book
-
-
-@pytest.mark.asyncio
-async def test_amending_record():
-    book = await Book(title='Neurodancer', author='William Gibson').save()
-    assert book.current_revision == 0
-    book.title = 'Neuromancer'
-    book = await book.save()
-    assert book.title == 'Neuromancer'
-    assert len(book.revision_hashes) == 2
-    assert book.current_revision == 1
-    assert book.revision_hashes[0] == book.id_hash
-    assert book.revision_hashes[1] != book.id_hash
-    await asyncio.sleep(1)
-    old_book = await book.fetch_revision(rev_no=0)
-    old_timestamp = old_book.timestamp
-    assert old_book.title == 'Neurodancer'
-    new_book = await book.fetch_revision(rev_no=1)
-    assert new_book.title == 'Neuromancer'
-    assert new_book.timestamp > old_timestamp
-
-
-@pytest.mark.asyncio
-async def test_store_and_index_record_of_records():
-    books = await asyncio.gather(
-        Book(title='Atlas Shrugged', author='Ayn Rand').save(),
-        Book(title='The Martian', author='Andy Weir').save()
-    )
-    new_library = await Library(name='The Library', books=books).save()
-    await asyncio.sleep(1)
-    fetched_library = await Library.where_eq(name='The Library').first()
-    assert new_library == fetched_library
-
-
-@pytest.mark.asyncio
-async def test_forget_object():
-    forgettable_book = await Book(title="The Forgotten Book", author="Mechthild Gläser").save()  # I'm sorry.
-    await asyncio.sleep(1)
-    await forgettable_book.forget()
-    assert forgettable_book.forgotten is True
-    await asyncio.sleep(1)
-    assert len(await Book.fetch(forgettable_book.id_hash).all()) == 0
-    with pytest.raises(AlreadyForgottenError):
-        await forgettable_book.forget()
-
-
-@pytest.mark.asyncio
-async def test_store_and_wrong_where_eq():
-    new_book = await Book(title='Atlas Shrugged', author='Ayn Rand').save()
-    assert new_book.title == 'Atlas Shrugged'
-    assert new_book.author == 'Ayn Rand'
-    with pytest.warns(UserWarning):
-        fetched_book = (await Book.where_eq(title='Atlas Shrugged', foo="bar").all())
-    assert len(fetched_book) == 0
-
-
-@pytest.mark.asyncio
-async def test_fetch_all_pagination():
-    page_one = await Book.fetch_objects().page(1, 1)
-    page_two = await Book.fetch_objects().page(2, 1)
-    assert len(page_one) == 1
-    assert len(page_two) == 1
-    assert page_one[0] != page_two[0]
-
-
-@pytest.mark.asyncio
-@pytest.mark.skip(reason="Only if you want to forget everything")
-async def test_drop_table():
-    await Record.forget_all()
-    assert len(await Book.fetch_objects().all()) == 0
-    assert len(await Library.fetch_objects().all()) == 0
-
-
-@pytest.mark.asyncio
-@pytest.mark.skip(reason="This takes a long time")
-async def test_sync_indices():
-    await AARS.sync_indices()
-    assert len(Record.get_indices()) == 3
-    assert len(Book.get_indices()) == 2
-    assert len(Library.get_indices()) == 1
-    assert len(list(Book.get_indices()[0].hashmap.values())) > 0
-    assert len(list(Book.get_indices()[1].hashmap.values())) > 0
-    assert len(list(Library.get_indices()[0].hashmap.values())) > 0
-
-
-@pytest.mark.asyncio
-async def test_empty_record_save():
-    class EmptyRecord(Record):
-        pass
-
-    with pytest.raises(ValueError):
-        await EmptyRecord().save()
-
-
-@pytest.mark.asyncio
-async def test_dict_field_save():
-    class BookWithDictAuthor(Record):
-        title: str
-        author: dict
-
-    book = await BookWithDictAuthor(title='Test Book', author={'first': 'John', 'last': 'Doe'}).save()
-    fetched_book = await BookWithDictAuthor.fetch(book.id_hash).first()
-    assert fetched_book.author == {'first': 'John', 'last': 'Doe'}
-
-
-@pytest.mark.asyncio
-async def test_negative_limit_pagination():
-    with pytest.raises(ValueError):
-        await Book.fetch_objects().page(1, -1)
-
-
-@pytest.mark.asyncio
-async def test_large_page_size_pagination():
-    page = await Book.fetch_objects().page(1, 100)
-    assert len(page) <= 100
-
-
-@pytest.mark.asyncio
-async def test_non_existent_revision():
-    book = await Book(title='Test Book', author='John Doe').save()
-    with pytest.raises(KeyError):
-        await book.fetch_revision(rev_no=10)
-
-
-@pytest.mark.asyncio
-async def test_save_without_changes():
-    book = await Book(title='Test Book', author='John Doe').save()
-    original_revision_count = len(book.revision_hashes)
-    book = await book.save()
-    assert len(book.revision_hashes) == original_revision_count
+import asyncio
+from typing import List, Optional
+
+from aleph.sdk import AuthenticatedAlephClient
+from aleph.sdk.conf import settings
+from aleph.sdk.chains.ethereum import get_fallback_account
+
+from src.aars import Record, Index, AARS
+from src.aars.exceptions import AlreadyForgottenError
+import pytest
+
+AARS(session=AuthenticatedAlephClient(get_fallback_account(), settings.API_HOST))
+
+
+@pytest.fixture(scope="session")
+def event_loop():
+    yield AARS.session.http_session.loop
+    asyncio.run(AARS.session.http_session.close())
+
+
+@pytest.fixture(scope="session", autouse=True)
+def create_indices(request):
+    Index(Book, "title")
+    Index(Book, ["title", "author"])
+    Index(Library, on="name")
+
+
+class Book(Record):
+    title: str
+    author: str
+    year: Optional[int]
+
+
+class Library(Record):
+    name: str
+    books: List[Book]
+
+
+def test_invalid_index_created():
+    try:
+        index = None
+        with pytest.raises(KeyError):
+            index = Index(Book, "some_nonexistent_field")
+    finally:
+        if index:
+            Record.remove_index(index)
+
+
+def test_duplicate_index_creation():
+    with pytest.raises(ValueError):
+        Index(Book, "title")
+
+
+@pytest.mark.asyncio
+async def test_sync_indices():
+    await AARS.sync_indices()
+    assert len(Record.get_indices()) == 3
+    assert len(Book.get_indices()) == 2
+    assert len(Library.get_indices()) == 1
+
+
+@pytest.mark.asyncio
+async def test_store_and_index():
+    new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
+    assert new_book.title == "Atlas Shrugged"
+    assert new_book.author == "Ayn Rand"
+    await asyncio.sleep(1)
+    fetched_book = await Book.where_eq(title="Atlas Shrugged").first()
+    assert new_book == fetched_book
+
+
+@pytest.mark.asyncio
+async def test_multi_index():
+    new_book = await Book(title="Lila", author="Robert M. Pirsig", year=1991).save()
+    # wait a few secs
+    await asyncio.sleep(1)
+    should_be_none = await Book.where_eq(title="Lila", author="Yo Momma").all()
+    assert len(should_be_none) == 0
+    fetched_book = await Book.where_eq(title="Lila", author="Robert M. Pirsig").first()
+    assert new_book == fetched_book
+
+
+@pytest.mark.asyncio
+async def test_amending_record():
+    book = await Book(title="Neurodancer", author="William Gibson").save()
+    assert book.current_revision == 0
+    book.title = "Neuromancer"
+    book = await book.save()
+    assert book.title == "Neuromancer"
+    assert len(book.revision_hashes) == 2
+    assert book.current_revision == 1
+    assert book.revision_hashes[0] == book.id_hash
+    assert book.revision_hashes[1] != book.id_hash
+    await asyncio.sleep(1)
+    old_book = await book.fetch_revision(rev_no=0)
+    old_timestamp = old_book.timestamp
+    assert old_book.title == "Neurodancer"
+    new_book = await book.fetch_revision(rev_no=1)
+    assert new_book.title == "Neuromancer"
+    assert new_book.timestamp > old_timestamp
+
+
+@pytest.mark.asyncio
+async def test_store_and_index_record_of_records():
+    books = await asyncio.gather(
+        Book(title="Atlas Shrugged", author="Ayn Rand").save(),
+        Book(title="The Martian", author="Andy Weir").save(),
+    )
+    new_library = await Library(name="The Library", books=books).save()
+    await asyncio.sleep(1)
+    fetched_library = await Library.where_eq(name="The Library").first()
+    assert new_library == fetched_library
+
+
+@pytest.mark.asyncio
+async def test_forget_object():
+    forgettable_book = await Book(
+        title="The Forgotten Book", author="Mechthild Gläser"
+    ).save()  # I'm sorry.
+    await asyncio.sleep(1)
+    await forgettable_book.forget()
+    assert forgettable_book.forgotten is True
+    await asyncio.sleep(1)
+    assert len(await Book.fetch(forgettable_book.id_hash).all()) == 0
+    with pytest.raises(AlreadyForgottenError):
+        await forgettable_book.forget()
+
+
+@pytest.mark.asyncio
+async def test_store_and_wrong_where_eq():
+    new_book = await Book(title="Atlas Shrugged", author="Ayn Rand").save()
+    assert new_book.title == "Atlas Shrugged"
+    assert new_book.author == "Ayn Rand"
+    with pytest.warns(UserWarning):
+        fetched_book = await Book.where_eq(title="Atlas Shrugged", foo="bar").all()
+    assert len(fetched_book) == 0
+
+
+@pytest.mark.asyncio
+async def test_fetch_all_pagination():
+    page_one = await Book.fetch_objects().page(1, 1)
+    page_two = await Book.fetch_objects().page(2, 1)
+    assert len(page_one) == 1
+    assert len(page_two) == 1
+    assert page_one[0] != page_two[0]
+
+
+@pytest.mark.asyncio
+async def test_dict_field_save():
+    class BookWithDictAuthor(Record):
+        title: str
+        author: dict
+
+    book = await BookWithDictAuthor(
+        title="Test Book", author={"first": "John", "last": "Doe"}
+    ).save()
+    fetched_book = await BookWithDictAuthor.fetch(book.id_hash).first()
+    assert fetched_book.author == {"first": "John", "last": "Doe"}
+
+
+@pytest.mark.asyncio
+async def test_negative_limit_pagination():
+    with pytest.raises(ValueError):
+        await Book.fetch_objects().page(1, -1)
+
+
+@pytest.mark.asyncio
+async def test_large_page_size_pagination():
+    page = await Book.fetch_objects().page(1, 100)
+    assert len(page) <= 100
+
+
+@pytest.mark.asyncio
+async def test_non_existent_revision():
+    book = Book(title="Test Book", author="John Doe")
+    await book.save()
+    with pytest.raises(IndexError):
+        await book.fetch_revision(rev_no=10)
+
+
+@pytest.mark.asyncio
+async def test_save_without_changes():
+    book = await Book(title="Test Book", author="John Doe").save()
+    original_revision_count = len(book.revision_hashes)
+    book = await book.save()
+    assert len(book.revision_hashes) == original_revision_count
+
+
+@pytest.mark.asyncio
+async def test_drop_table():
+    await Record.forget_all()
```

### Comparing `aars-0.5.5b1/.gitignore` & `aars-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aars-0.5.5b1/LICENSE` & `aars-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aars-0.5.5b1/README.md` & `aars-0.5.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,109 @@
-#AARS - Aleph Asynchronous Record Storage
+Metadata-Version: 2.1
+Name: aars
+Version: 0.5.6
+Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
+Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
+Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
+Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# AARS - Aleph Active Record SDK
 AARS is a powerful and flexible Python library built on top of the Aleph decentralized storage network, designed to help you build better backends for your decentralized applications. It provides an easy-to-use interface for managing and querying your data, with a focus on performance and versatility.
 
-##Features
+## Features
 - Asynchronous, high-performance data storage and retrieval
 - Customizable schema with support for different data types
 - Indexing for efficient querying
 - Revision history tracking for records
 - Support for forgetting data (GDPR compliant)
 - Built-in pagination for large result sets
 
-##Installation
+## Installation
 Install AARS using pip:
 
 ```shell
 pip install aars
 ```
 
-##Getting Started
+## Getting Started
 To get started with AARS, you will need to define your data schema by creating classes that inherit from Record. These classes represent the objects you want to store and query on the Aleph network.
 
 Here's an example of how you can implement a simple social media platform, that we'll call "Chirper":
 
 ```python
-from src.aars import Record, Index
-from typing import List
+from src.aars import Record
 
 class User(Record):
     username: str
-    display_name: str
-    bio: Optional[str]
+    bio: str
 
 class Chirp(Record):
     author: User
     content: str
     likes: int
     timestamp: int
 ```
 In this example, we have a User class representing a user of Chirper, and a Chirp class representing a user's message. Now, let's create some indices to make querying our data more efficient:
 
 ```python
+from src.aars import Index
+
 Index(User, 'username')
 Index(Chirp, 'author')
 Index(Chirp, 'timestamp')
 ```
-With the schema defined and indices created, we can now perform various operations, such as creating new records, querying records, and updating records:
+With the schema defined and indices created, we only need to initialize an AARS session:
+    
+```python
+from src.aars import AARS
+
+AARS()
+```
+It is enough to call the constructor once, and it will automatically initialize the session with the default settings.
+
+We can now perform various operations, such as creating new records, querying records, and updating records:
 
 ```python
+import time
+
 # Create a new user
 new_user = await User(username='chirpy_user', display_name='Chirpy User', bio='I love chirping!').save()
 
 # Create a new chirp
 new_chirp = await Chirp(author=new_user, content='Hello, Chirper!', likes=0, timestamp=int(time.time())).save()
 
 # Query chirps by author
 chirps_by_author = await Chirp.where_eq(author=new_user).all()
 
 # Update a chirp
 new_chirp.likes += 1
 updated_chirp = await new_chirp.save()
 ```
 
-##Documentation
-For detailed documentation, including advanced features such as revision history, forgetting data, and pagination, refer to the docs folder in the repository or visit the official documentation website.
+## Documentation
+For detailed documentation, including advanced features such as revision history, forgetting data, and pagination,
+refer to the docs folder in the repository or [visit the official documentation website](https://aleph-im.github.io/active-record-sdk/).
+
+## Building the Docs
+To build the documentation, you will need to install the dependencies listed in the requirements.txt and docs-requirements.txt. Then, run the following command:
+
+```shell
+mkdocs build
+```
+
+You can serve the documentation locally by running the following command:
+
+```shell
+mkdocs serve
+```
 
-##Contributing
+## Contributing
 Contributions to AARS are welcome! If you have found a bug, want to suggest an improvement, or have a question, feel free to open an issue on the GitHub repository.
 
-##License
-AARS is released under the MIT License.
+## License
+AARS is released under the [MIT License](https://github.com/aleph-im/active-record-sdk/blob/main/LICENSE).
```

### Comparing `aars-0.5.5b1/pyproject.toml` & `aars-0.5.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "aars"
-version = "0.5.5-beta.1"
-authors = [
-  { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
-]
-description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[dependencies]
-pydantic = "^1.8.2"
-aleph-sdk-python = "^0.6.0"
-
-[project.urls]
-"Homepage" = "https://github.com/aleph-im/active-record-sdk"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "aars"
+version = "0.5.6"
+authors = [
+  { name="Mike Hukiewitz", email="mike.hukiewitz@robotter.ai" },
+]
+description = "Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[dependencies]
+pydantic = "^1.8.2"
+aleph-sdk-python = "^0.6.0"
+
+[project.urls]
+"Homepage" = "https://github.com/aleph-im/active-record-sdk"
 "Bug Tracker" = "https://github.com/aleph-im/active-record-sdk/issues"
```

### Comparing `aars-0.5.5b1/PKG-INFO` & `aars-0.5.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,95 @@
-Metadata-Version: 2.1
-Name: aars
-Version: 0.5.5b1
-Summary: Experimental Object-Document-Mapper using pydantic to store objects on Aleph.im
-Project-URL: Homepage, https://github.com/aleph-im/active-record-sdk
-Project-URL: Bug Tracker, https://github.com/aleph-im/active-record-sdk/issues
-Author-email: Mike Hukiewitz <mike.hukiewitz@robotter.ai>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-#AARS - Aleph Asynchronous Record Storage
-AARS is a powerful and flexible Python library built on top of the Aleph decentralized storage network, designed to help you build better backends for your decentralized applications. It provides an easy-to-use interface for managing and querying your data, with a focus on performance and versatility.
-
-##Features
-- Asynchronous, high-performance data storage and retrieval
-- Customizable schema with support for different data types
-- Indexing for efficient querying
-- Revision history tracking for records
-- Support for forgetting data (GDPR compliant)
-- Built-in pagination for large result sets
-
-##Installation
-Install AARS using pip:
-
-```shell
-pip install aars
-```
-
-##Getting Started
-To get started with AARS, you will need to define your data schema by creating classes that inherit from Record. These classes represent the objects you want to store and query on the Aleph network.
-
-Here's an example of how you can implement a simple social media platform, that we'll call "Chirper":
-
-```python
-from src.aars import Record, Index
-from typing import List
-
-class User(Record):
-    username: str
-    display_name: str
-    bio: Optional[str]
-
-class Chirp(Record):
-    author: User
-    content: str
-    likes: int
-    timestamp: int
-```
-In this example, we have a User class representing a user of Chirper, and a Chirp class representing a user's message. Now, let's create some indices to make querying our data more efficient:
-
-```python
-Index(User, 'username')
-Index(Chirp, 'author')
-Index(Chirp, 'timestamp')
-```
-With the schema defined and indices created, we can now perform various operations, such as creating new records, querying records, and updating records:
-
-```python
-# Create a new user
-new_user = await User(username='chirpy_user', display_name='Chirpy User', bio='I love chirping!').save()
-
-# Create a new chirp
-new_chirp = await Chirp(author=new_user, content='Hello, Chirper!', likes=0, timestamp=int(time.time())).save()
-
-# Query chirps by author
-chirps_by_author = await Chirp.where_eq(author=new_user).all()
-
-# Update a chirp
-new_chirp.likes += 1
-updated_chirp = await new_chirp.save()
-```
-
-##Documentation
-For detailed documentation, including advanced features such as revision history, forgetting data, and pagination, refer to the docs folder in the repository or visit the official documentation website.
-
-##Contributing
-Contributions to AARS are welcome! If you have found a bug, want to suggest an improvement, or have a question, feel free to open an issue on the GitHub repository.
-
-##License
-AARS is released under the MIT License.
+# AARS - Aleph Active Record SDK
+AARS is a powerful and flexible Python library built on top of the Aleph decentralized storage network, designed to help you build better backends for your decentralized applications. It provides an easy-to-use interface for managing and querying your data, with a focus on performance and versatility.
+
+## Features
+- Asynchronous, high-performance data storage and retrieval
+- Customizable schema with support for different data types
+- Indexing for efficient querying
+- Revision history tracking for records
+- Support for forgetting data (GDPR compliant)
+- Built-in pagination for large result sets
+
+## Installation
+Install AARS using pip:
+
+```shell
+pip install aars
+```
+
+## Getting Started
+To get started with AARS, you will need to define your data schema by creating classes that inherit from Record. These classes represent the objects you want to store and query on the Aleph network.
+
+Here's an example of how you can implement a simple social media platform, that we'll call "Chirper":
+
+```python
+from src.aars import Record
+
+class User(Record):
+    username: str
+    bio: str
+
+class Chirp(Record):
+    author: User
+    content: str
+    likes: int
+    timestamp: int
+```
+In this example, we have a User class representing a user of Chirper, and a Chirp class representing a user's message. Now, let's create some indices to make querying our data more efficient:
+
+```python
+from src.aars import Index
+
+Index(User, 'username')
+Index(Chirp, 'author')
+Index(Chirp, 'timestamp')
+```
+With the schema defined and indices created, we only need to initialize an AARS session:
+    
+```python
+from src.aars import AARS
+
+AARS()
+```
+It is enough to call the constructor once, and it will automatically initialize the session with the default settings.
+
+We can now perform various operations, such as creating new records, querying records, and updating records:
+
+```python
+import time
+
+# Create a new user
+new_user = await User(username='chirpy_user', display_name='Chirpy User', bio='I love chirping!').save()
+
+# Create a new chirp
+new_chirp = await Chirp(author=new_user, content='Hello, Chirper!', likes=0, timestamp=int(time.time())).save()
+
+# Query chirps by author
+chirps_by_author = await Chirp.where_eq(author=new_user).all()
+
+# Update a chirp
+new_chirp.likes += 1
+updated_chirp = await new_chirp.save()
+```
+
+## Documentation
+For detailed documentation, including advanced features such as revision history, forgetting data, and pagination,
+refer to the docs folder in the repository or [visit the official documentation website](https://aleph-im.github.io/active-record-sdk/).
+
+## Building the Docs
+To build the documentation, you will need to install the dependencies listed in the requirements.txt and docs-requirements.txt. Then, run the following command:
+
+```shell
+mkdocs build
+```
+
+You can serve the documentation locally by running the following command:
+
+```shell
+mkdocs serve
+```
+
+## Contributing
+Contributions to AARS are welcome! If you have found a bug, want to suggest an improvement, or have a question, feel free to open an issue on the GitHub repository.
+
+## License
+AARS is released under the [MIT License](https://github.com/aleph-im/active-record-sdk/blob/main/LICENSE).
```

