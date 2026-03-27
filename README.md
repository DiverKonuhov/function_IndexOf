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
№ неудачные варианты
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
