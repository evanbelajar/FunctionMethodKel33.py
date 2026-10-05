class TaskManager:
    def __init__(self):
        self.tasks = []

    # Method non-return type dengan parameter, untuk menambah tugas
    def add_task(self, task):
        if task:
            self.tasks.append(task)
            print(f"Tugas '{task}' berhasil ditambahkan.")
        else:
            print("Tugas tidak boleh kosong!")

    # Method non-return type tanpa parameter, untuk menampilkan semua tugas
    def display_tasks(self):
        if not self.tasks:
            print("Belum ada tugas.")
        else:
            print("Daftar Tugas:")
            for idx, task in enumerate(self.tasks, 1):
                print(f"{idx}. {task}")

# Fungsi return type dengan parameter, menghitung jumlah kata dalam sebuah string tugas
def count_words(task: str) -> int:
    return len(task.split()) if task else 0

# Fungsi return type tanpa parameter, memberikan pesan pembuka
def welcome_message() -> str:
    return "Selamat datang di Task Manager!\n"

# Fungsi non-return type tanpa parameter, menampilkan pesan penutup
def goodbye_message():
    print("Terima kasih telah menggunakan Task Manager. Sampai jumpa!")

# Program utama
print(welcome_message())

manager = TaskManager()

tasks_to_add = ["Belajar Python", "Mengerjakan tugas modul 3", "Baca buku tentang algoritma"]

for task in tasks_to_add:
    if len(task) > 5:  # pengkondisian: hanya tambah jika panjang string lebih dari 5
        manager.add_task(task)

manager.display_tasks()

# Contoh penggunaan fungsi dengan return untuk menghitung kata di tugas pertama
if manager.tasks:
    kata = count_words(manager.tasks[0])
    print(f"Tugas pertama memiliki {kata} kata.")

goodbye_message()
