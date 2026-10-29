#include <iostream>
using namespace std;

int main() {
    setlocale(LC_ALL, "Russian");

    int N, seat;
    cout << "Введите N (1-100): ";
    cin >> N;

    if (N < 1 || N > 100) {
        cout << "Ошибка: недопустимое N" << endl;
        return 1;
    }

    int count = 0;
    int matches = 0;
    int previous_seat = -1;

    while (true) {
        cout << "Введите место (0 to stop): ";
        cin >> seat;

        if (seat == 0) {
            break;
        }

        if (seat >= 1 && seat <= N) {
            count++;

            if (previous_seat == seat) {
                matches++;
            }

            previous_seat = seat;
        }
    }

    cout << "Принято записей: " << count << endl;
    cout << "Совпадений с предыдущим: " << matches << endl;

    return 0;
}
