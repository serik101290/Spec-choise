Console.Clear();
// Запрашиваем у пользователя строку с разделенными запятой словами
Console.WriteLine("Введите слова через запятую:");
string input = Console.ReadLine();

// Разбиваем строку на отдельные слова и помесщаем их в массив
string[] words = input.Split(new char[] { ',', ' ' }, StringSplitOptions.RemoveEmptyEntries);

// Выводим только те строки, которые содержат слова длиной 3 и менее
Console.WriteLine("Строки, содержащие слова длиной 3 и менее:");
for (int i = 0; i < words.Length; i++)

{
    if (words[i].Length <= 3)
        {
            Console.WriteLine(words[i]);
        }
}

// Ждем нажатия клавиши перед завершением программы
Console.ReadKey();