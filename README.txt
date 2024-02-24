File frontend menampilkan api dari cat ninja facts, untuk websitenya, tampilin cat factsnya bisa lama tergantung internet


Yang backend mengambil data dari server MySQL, restoran_db
CREATE DATABASE restoran_db;
USE restoran_db;
CREATE TABLE customers (
    ->     customer_id INT AUTO_INCREMENT PRIMARY KEY,
    ->     customer_name VARCHAR(255),
    ->     email VARCHAR(255),
    ->     city VARCHAR(255)
    -> );
CREATE TABLE orders (
    ->     order_id INT AUTO_INCREMENT PRIMARY KEY,
    ->     customer_id INT,
    ->     total_amount DECIMAL(10, 2),
    ->     FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
    -> );

Yang backend json mengambil data dari json yang ada di file tersebut, namun fungsi sama seperti backend

