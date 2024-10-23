# Programowanie
Lessons
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ProjectNr1_Khomenko_71506
{
    internal class Program
    {
        static void Main(string[] args)
        {
            // deklaracja zmiennej identyfik. naciśninie klawisz
            ConsoleKeyInfo WybranaFunkcjonalność;

            // wypisanie Metryki programu
            Console.WriteLine("\n\n\t\t\t\tPROGRAM KALKULATOR umożliwia obliczanie wartości wybranych wielkości matematycznych");

            // zapisanie wielokrotnego powtarzania wysołań kalkulatorów
            do
            {
                // wypisanie MENU części głównej
                Console.WriteLine("\n\n\t\tMENU części głównej progamu");
                // wypisanie kolejbej pozycji MENU programu
                Console.WriteLine("\n\t\tA. Kalkulator laboratoryjny");
                Console.WriteLine("\n\t\tB. Kalkulator Indywidualny");
                Console.WriteLine("\n\t\tX. Zakońć programę");
                // wypisanie odpowiedzi dla użytkownika
                Console.Write("\n\n\t\tNaciśnij jeden z dozwolonych klawiszy (A, B, X) dla wybrania wymaganej funkcjonalności: ");
                // wczytanie kodu naciśnietego klawisza (wybranej funcjonalności)
                WybranaFunkcjonalność = Console.ReadKey();
                // rozpoznanie wybranej funkconalności
                if (WybranaFunkcjonalność.Key == ConsoleKey.A)
                    // został wybrany kalkulator Laboratoryjny
                    KalkulatorLaboratoryjny();
                else
                    if (WybranaFunkcjonalność.Key == ConsoleKey.B)
                    // został wybrany Kalkulator Indywidualny 
                    KalkulatorIndywidualny();
                else
                    if (WybranaFunkcjonalność.Key != ConsoleKey.X)
                    // Eror
                    Console.WriteLine("Niezadowolny znak");

                // wyczyszczenie okna konsoli 
                Console.Clear();

            } while (WybranaFunkcjonalność.Key != ConsoleKey.X);
            // chwilowe zatrzymanie
            Console.WriteLine("Autor programu: Oleksandr Khomenko");
            // data urochomienia
            Console.WriteLine("\n\t\tDzisiejsza data: {0}", DateTime.Now);
            Console.Write("\n\n\n\t\tNaciśnij dowolny klawisz dla kontynuacji...");
            Console.ReadKey();
        } // od Main
        #region Deklaracje metod z Kalkulatorami 
        static void KalkulatorLaboratoryjny()
        {
            // deklaracja zmiennej identyfik. naciśninie klawisz
            ConsoleKeyInfo WybranaFunkcjonalność;
            Console.Clear();
            // wilekorotne powtarzanie obliczań wielkości matematycznych
            do
            {
                // wypisanie Metryki Kalkulatora Laboratoryjnego
                Console.WriteLine("\n\n\n\t\tMEENU Kalkulatora Laboratoryjnego");
                Console.WriteLine("\n\n\t\tA. Obliczenie średnej arytmetycznej wyrazów ciągu liczbowego");
                Console.WriteLine("\n\n\t\tB. Obliczenie wartości wielomianu n-tego stopnia");
                Console.WriteLine("\n\n\t\tC. Obliczenie konwersji znakowego zapisu liczby na wartość");
                Console.WriteLine("\n\n\t\tD. Obliczenie wartości symbolu Newtona");
                Console.WriteLine("\n\t\tX. Wyjście z kalkulatora Laboratoryjnego");
                // wypisanie odpowiedzi dla Użytkownika
                Console.Write("\n\n\tNaciśnij dozwolony klawisz (A, B, C, D i X) dla wybrania jednej z oferowanych wunkcjonalności: ");
                // wczytanie kodu naciśniętego klawisza
                WybranaFunkcjonalność = Console.ReadKey();
                //rozpoznanie wybranej funkcjonalmości
                switch (WybranaFunkcjonalność.Key)
                {
                    case ConsoleKey.A: //potwierdzenie wybranej funkcjonalności
                        Console.WriteLine("\n\n\t Wybrałeś funkcjonalność: A. Obliczenie średnej arytmetycznej wyrazów ciągu liczbowego");
                        Console.WriteLine("\n\n\t\tPRZEPRASZAM, ale jestem w trkcie projektowania");
                        break;
                    case ConsoleKey.B: 
                        Console.WriteLine("\n\n\t Wybrałeś funkcjonalność: B. Obliczenie wartości wielomianu n-tego stopnia");
                        Console.WriteLine("\n\n\t\tPRZEPRASZAM, ale jestem w trkcie projektowania");
                        break;
                    case ConsoleKey.C: 
                        Console.WriteLine("\n\n\t Wybrałeś funkcjonalność: C. Obliczenie konwersji znakowego zapisu liczby na wartość");
                        Console.WriteLine("\n\n\t\tPRZEPRASZAM, ale jestem w trkcie projektowania");
                        break;
                    case ConsoleKey.D: 
                        Console.WriteLine("\n\n\t Wybrałeś funkcjonalność: D. Obliczenie wartości symbolu Newtona");
                        Console.WriteLine("\n\n\t\tPRZEPRASZAM, ale jestem w trkcie projektowania");
                        break;
                    case ConsoleKey.X:
                        Console.WriteLine("\n\n\t Wybrałeś X. Wyjście z kalkulatora Laboratoryjnego");
                        break;
                        default: Console.WriteLine("\n\n\t\tError: nacisnąłeś niedozwolony znak");
                        break;
                }


            } while (WybranaFunkcjonalność.Key != ConsoleKey.X);
            // wypisanie komunikatu
            Console.WriteLine("\n\n\n\t\tPRZEPRASZAM, ale jestem w trakcie realizacji (implementacji)");
            Console.Write("\n\n\n\t\tNaciśnij dowolny klawisz dla kontynuacji...");
            Console.ReadKey();
            Console.Clear();
        }

        static void KalkulatorIndywidualny()
        {
            // wypisanie komunikatu
            Console.WriteLine("\n\n\n\t\tPRZEPRASZAM, ale jestem w trakcie realizacji (implementacji)");
            Console.Write("\n\n\n\t\tNaciśnij dowolny klawisz dla kontynuacji...");
            Console.ReadKey();
        }
        #endregion
    }
}
