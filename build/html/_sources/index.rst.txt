.. week 5 döküm documentation master file, created by
   sphinx-quickstart on Mon May 12 23:34:43 2025.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to week 5 döküm's documentation!

Sections
--------

Sections
========

1. Image processing assignment …  
2. Georeferencing with QGIS …  
3. GNSS satellite position calculation …  
4. Bubble Sort implementation

   .. code-block:: python

      def bubble_sort(arr):
          n = len(arr)
          for i in range(n):
              swapped = False
              for j in range(0, n - i - 1):
                  if arr[j] > arr[j + 1]:
                      arr[j], arr[j + 1] = arr[j + 1], arr[j]
                      swapped = True
              if not swapped:
                  break
          return arr

      if __name__ == "__main__":
          data = [5, 2, 9, 1, 5, 6]
          print("Original:", data)
          print("Sorted:  ", bubble_sort(data.copy()))

========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

    goruntu_isleme
    buuble_sort 

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
