# stunning-octo-memory2
lab6-
await authorsCollection.insertMany([
  { name: "Тарас Шевченко", birth_year: 1814, nationality: "український" },
  { name: "Леся Українка", birth_year: 1871, nationality: "український" }
]);

await booksCollection.insertMany([
  {
    title: "Кобзар",
    author: "Тарас Шевченко",
    publication_year: 1840,
    genres: ["поезія", "романтизм"],
    available: true
  },
  {
    title: "Лісова пісня",
    author: "Леся Українка",
    publication_year: 1911,
    genres: ["драма", "феєрія"],
    available: true
  }
]);

await usersCollection.insertMany([
  { username: "ivan_petrov", borrowed_books: ["Кобзар"], status: "active" },
  { username: "maria_kovalenko", borrowed_books: [], status: "active" }
]);
