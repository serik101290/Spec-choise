Console.Clear();
// Запрашиваем у пользователя строку с разделенными запятой словами
Console.WriteLine("Введите слова через запятую:");
string input = Console.ReadLine();

// Разбиваем строку на отдельные слова и помесщаем их в массив
string[] words = input.Split(new char[] { ',', ' ' }, StringSplitOptions.RemoveEmptyEntries);
