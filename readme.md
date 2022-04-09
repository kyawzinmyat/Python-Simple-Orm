Orm project hasn't finished yet
this project  inspire gtback orm video

you can create database object and create table by passing table object!


You can now insert values into table!

You can query now 

You can now add foreign key
You can now update
_____________________________________________


Api 

db = Database() this will create sqlite.db in current dir.
db.table() that will return the names of table in the database
db.save()  like django orm that will do two things depending on the instancem
db.drop(Table name) that will delete table from database



Class Test(Table): Table is class
    Column_name = Column() Column is class 

db.create(Test) that will create table with name class name and column with its attribute

test1 = Test(Column_name="test") if you set invalid column that will raise value error
db.save(test1) that will insert Column_name value into Test tale


test1.all() that will return the object of every row
test1.get(column_name=value) that will return specific object

test1 = Test1.get(id=1) that wil return Test object with attribute Column_name="test"

test1.Column_name = "Changed"
db.save(test1) now this save is for update

The way save implemented is the same as django documentation explain
.It say save does two thing depending on the conditions.
Current save method will be updated every field even if it doesn't change in value.
Foreign key work the same way!!

