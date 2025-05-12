Bubble Sort Algoritması
=======================

Bu bölümde, geçen hafta incelediğimiz **Bubble Sort** sıralama algoritmasının mantığını, Python kodunu ve test örneklerini bulabilirsiniz.

Algoritma Özeti
---------------

1. Listenin başından sonuna kadar ilerleyin.
2. Her komşu çifti karşılaştırın; eğer önceki eleman büyükse, yer değiştirin.
3. Bir tur boyunca hiçbir değişiklik yapılmadıysa, sıralama tamamlanmıştır.

Kod Örneği
----------

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

Test Örneği
-----------

.. code-block:: python

   if __name__ == "__main__":
       data = [5, 2, 9, 1, 5, 6]
       sorted_data = bubble_sort(data.copy())
       print("Orijinal:", data)
       print("Sıralı:  ", sorted_data)

