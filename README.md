a. How much data will the publisher send in one run?
Publisher akan mengirim 5 events ke message broker dalam sekali run. Setiap event berisi data UserCreatedEventMessage dengan field user_id dan user_name. Jadi total ada 5 pesan yang dikirim ke queue user_created.

b. The url "amqp://guest:guest@localhost:5672" is the same as in subscriber, what does it mean?
Artinya publisher dan subscriber terhubung ke message broker yang sama. Keduanya menggunakan username guest, password guest, dan terhubung ke RabbitMQ yang berjalan di localhost port 5672. Inilah yang memungkinkan publisher mengirim event dan subscriber menerimanya.