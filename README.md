# Python_homework_3
Homework Python

Импорт random

    import random
1. Генерация списка из 500 Emails

       emails_list = [f"user_{i}@gmail.com" for i in range(1, 501)]
2. Преобразование списка Emails в Dict с использованием индекса

       emails_dict = {index: email for index, email in enumerate(emails_list)}
3. Создание списка Name_Surname из 100 элементов с именем "Adam" каждое 10-е имя

       name_surname_list = [f"Adam_{i}" if (i + 1) % 10 == 0 else f"Other_{i}" for i in range(100)]
4. Создание списка списков с парами Adam-ов и Eva-фамилий

       adam_eva_pairs = [[name, f"Eva_{name.split('_')[1]}"] for name in name_surname_list if name.startswith("Adam")]
5. Генерация списка из 100 кличек для животных с 10 одинаковыми кличками

       animal_names_list = ["Spike", "Barboss", "Bloom"] * 10
6. Удаление дубликатов из списка кличек

       unique_animal_names = list(set(animal_names_list))
Вывод результатов

    print("1. Список Emails:", emails_list[:5], "...")
    print("\n2. Emails в виде Dict:", emails_dict)
    print("\n3. Список Name_Surname:", name_surname_list[:5], "...")
    print("\n4. Список Adam-Eva пар:", adam_eva_pairs[:2], "...")
    print("\n5. Список кличек для животных:", animal_names_list[:5], "...")
    print("\n6. Уникальные клички:", unique_animal_names[:5], "...")
