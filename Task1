#include <iostream>
using namespace std;
int main() {
    setlocale(LC_ALL, "Russian");
    int n, tickets;
    cout << "Введите количество сеансов (1-16): ";
    cin >> n;
    if (n < 1 || n > 16) {
        cout << "Ошибка: недопустимое количество сеансов" << endl;
        return 1;
    }
    int sum = 0;
    int max_sum = -1;
    int max_session = 0;
    for (int i = 1; i <= n; i++) {
        cout << "Сеанс " << i << " билеты (0-100): ";
        cin >> tickets;
        if (tickets < 0 || tickets > 100) {
            cout << "Ошибка: недопустимое количество билетов" << endl;
            return 1;
        }
        int price;
        if (i % 2 != 0) {
            price = 8;
        }
        else {
            price = 10;
        }
        int sess_sum = tickets * price;
        cout << "Сеанс " << i << " выручка: " << sess_sum << endl;
        sum = sum + sess_sum;
        if (sess_sum > max_sum) {
            max_sum = sess_sum;
            max_session = i;
        }
    }
    cout << "Общая выручка: " << sum << endl;
    cout << "Сеанс с максимальной выпучкой: " << max_session << endl;

    return 0;
}
