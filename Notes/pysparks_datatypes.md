[Home Page](README.md)

# PySpark Data Types

In PySpark, data types define the type of data that can be stored in a DataFrame column. Here is a list of common PySpark data types with examples:

## Primitive Data Types

1. **StringType** - String data type.
   - Example: `"Hello, world!"`
   - Explanation: This is similar to a `str` in Python.

2. **IntegerType** - Integer data type.
   - Example: `42`
   - Explanation: This is similar to an `int` in Python.

3. **LongType** - Long integer data type.
   - Example: `9223372036854775807`
   - Explanation: This is similar to a `long` in Python 2, but in Python 3, it's just `int`.

4. **FloatType** - Float data type.
   - Example: `3.14`
   - Explanation: This is similar to a `float` in Python.

5. **DoubleType** - Double data type.
   - Example: `3.141592653589793`
   - Explanation: This represents double-precision floating-point numbers, similar to `float` in Python but with more precision.

6. **ShortType** - Short integer data type.
   - Example: `32767`
   - Explanation: This is an integer type that is smaller in range, similar to `short` in other programming languages, but not directly present in Python.

7. **ByteType** - Byte data type.
   - Example: `127`
   - Explanation: This represents a small integer, similar to a byte-sized integer in other languages, but not directly present in Python.

8. **BinaryType** - Binary data type (byte array).
   - Example: `b'\x01\x02\x03'`
   - Explanation: This is similar to a `bytes` object in Python.

## Numeric Data Types

1. **DecimalType** - Fixed-point decimal data type.
   - Example: `Decimal('10.5')`
   - Explanation: This is similar to `decimal.Decimal` in Python for high-precision arithmetic.

2. **BooleanType** - Boolean data type (true or false).
   - Example: `True` or `False`
   - Explanation: This is similar to `bool` in Python.

## Date and Time Data Types

1. **DateType** - Date data type.
   - Example: `datetime.date(2023, 7, 7)`
   - Explanation: This is similar to `datetime.date` in Python.

2. **TimestampType** - Timestamp data type.
   - Example: `datetime.datetime(2023, 7, 7, 12, 34, 56)`
   - Explanation: This is similar to `datetime.datetime` in Python.

## Complex Data Types

1. **ArrayType** - Array data type.
   - Example: `[1, 2, 3]`
   - Explanation: This is similar to a `list` in Python.

2. **MapType** - Map data type (key-value pairs).
   - Example: `{'key1': 'value1', 'key2': 'value2'}`
   - Explanation: This is similar to a `dict` in Python.

3. **StructType** - Struct data type (collection of fields).
   - Example:
     ```python
     from pyspark.sql.types import StructType, StructField, StringType, IntegerType

     schema = StructType([
         StructField("name", StringType(), True),
         StructField("age", IntegerType(), True)
     ])
     ```
   - Explanation: This is similar to defining a class or a complex data structure with multiple fields in Python.

## Null Data Type

1. **NullType** - Null data type.
   - Example: `None`
   - Explanation: This is similar to `None` in Python.

These data types are used to define schema for DataFrames and to cast or convert between different types when necessary.

[Home Page](README.md)
