# function_IndexOf
от скуки написал функцию 



изначально меня неустроило то сколько ест памяти мой код для простого вывода небольшой инфы через консоль в итоге я пришёл этому ужасу 
var myVars = new Dictionary<string, int[]>();
myVars["King Balon the {}th has {} rooms"] = new int[] { 6, 102 };

Console.Write(Format(myVars.Keys.First(), myVars.Values.First()));
string Format(string template, int[] vals)
{
    string clone = template;
    foreach (var n in vals)
    {
        int pos = clone.IndexOf("{}");
        if (pos != -1) clone = clone.Remove(pos, 2).Insert(pos, n.ToString());
    }
    return clone;
}



Также хочу заметить что были и неудачные варианты но по большому счёту я потратил на эту фигню целый день
# неудачные варианты
var king = "King Balon the 6th";

// BEGIN (write your solution here)
//King Balon the 6th has 102 rooms.
var initializedNum = 6 initializedNum2 = 102;;
var cddd = $"""King Balon the {initializedNum}th has {initializedNum2} rooms""";
var myVars = new Dictionary<string, int>();
myVars[cddd] = 6;
Console.Write($"{myVars.Keys.First()}");
//другой код

var myVars = new Dictionary<string, int[]>();

// Сохраняем два числа: 6 (индекс 0) и 10 (индекс 1)
myVars[var cddd = $"""King Balon the {}th has {} rooms""";] = new int[] { 6, 10 }; 

// Достаем массив по ключу "King"
var values = myVars[cddd];

// Собираем строку, где 6 будет в начале, а 10 в конце
Console.Write($"{nameof(myVars[cddd[string.IndexOf('{')values[0], string.IndexOf('}'(поиск уже с конца а не с начала строки))values[1]]])}");
// END

# Так же ещё одна функция мне было скучно и я подумал непользоваться стрингами
//Создайте строку с текстом One more time, явно укажите тип данных и выведите ее на экран
int num1 = 0, num2 = 0;
char[,] matrix = new char[12, 12];

matrix[0, 0] = 'O'; matrix[0, 1] = 'n'; matrix[0, 2] = 'e'; matrix[0, 3] = '\0'; matrix[0, 4] = '\0'; matrix[0, 5] = ' ';
matrix[1, 0] = '\0'; matrix[1, 1] = 'm'; matrix[1, 2] = 'o'; matrix[1, 3] = 'r'; matrix[1, 4] = 'e'; matrix[1, 5] = ' ';
matrix[2, 0] = '\0'; matrix[2, 1] = 't'; matrix[2, 2] = 'i'; matrix[2, 3] = 'm'; matrix[2, 4] = 'e'; matrix[2, 5] = '\0';
matrix[3, 0] = '\0'; matrix[3, 1] = '\0'; matrix[3, 2] = '\0'; matrix[3, 3] = '\0'; matrix[3, 4] = '\0'; matrix[3, 5] = '\0';

for(int i = 0, j = 0; i<24 && j<4;)
{
    Console.Write(matrix[j, i]); 
    if(i == 6)
    {
        j++;
        i--;
        i--;
        i--;
        i--;
        i--;
        i--;
    }
    i++;

}

# рабочий вариант от нейросети без стрингов

