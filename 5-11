#include <iostream>
#include <vector>
#include <unordered_map>
using namespace std;

int main() {
    int n;
    cout << "Введите количество элементов в массиве: ";
    cin >> n;

    vector<int> array(n);
    cout << "Введите элементы массива:" << endl;
    for (int i = 0; i < n; ++i) {
        cin >> array[i];
    }

    unordered_map<int, int> frequency;

    for (int num : array) {
        frequency[num]++;
    }

    cout << "Повторяющиеся элементы:" << endl;
    bool found = false;

    for (const auto& pair : frequency) {
        if (pair.second >= 2) {
            cout << pair.first << " (повторяется " << pair.second << " раз(а))" << endl;
            found = true;
        }
    }

    if (!found) {
        cout << "Нет повторяющихся элементов." << endl;
    }

    return 0;
}
