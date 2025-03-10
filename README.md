using System;

namespace SimpleIntro
{
    class AboutMe
    {
        readonly string nickname = "Havoks";
        readonly bool isMale = true;
        readonly string[] skills = { "C#", "a new framework" };
        readonly string quote = "you are not anonymous here";

        public string Introduce()
        {
            return $"👋 Hi, I'm {nickname}!";
        }

        static void Main(string[] args)
        {
            AboutMe me = new AboutMe();
            Console.WriteLine(me.Introduce());
            Console.WriteLine($"Gender: {(me.isMale ? "Male" : "Female")}");
            Console.WriteLine($"🌍 Location: Vietnamese");
            Console.WriteLine($"🧠 Learning: {string.Join(", ", me.skills)}");
            Console.WriteLine($"⚡ Quote: {me.quote}");
        }
    }
}
