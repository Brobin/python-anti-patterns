Don't use just class
==========================

When you have a method that doesn't really needs a class to belong, don't create a new class just to put it inside. In Python we can create methods that don't belong to class. Furthermore, you can put in just one file a lot of methods that don't have any class.

Example
-------

The ``DateUtil`` class below has the ``convert`` method that transform a weekday from datetime to weekday in the string form.

.. code:: python

    class DateUtil:
        @staticmethod
        def from_weekday_to_string(weekday):
            nameds_weekdays = {
                0: 'Monday',
                5: 'Friday'
            }

            return nameds_weekdays[weekday]

It's not necessary create a class to do this. You could just create a new file to put it, or put it in an exists one.

Solutions
-----------
Puting the method outside of the class.
..........................................................


.. code:: pyton
# file date_utils.py

def from_weekday_to_string(weekday):
    nameds_weekdays = {
        0: 'Monday',
        5: 'Friday'
    }

    return nameds_weekdays[weekday]

References
----------
