# SQLodev8
## sql sorguları patika odev 8 ##
1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.<br/><br/>
CREATE TABLE employee (<br/>
    id SERIAL PRIMARY KEY,<br/>
    name VARCHAR(50),<br/>
    birthday DATE,<br/>
    email VARCHAR(100)<br/>
);<br/><br/><br/>
3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.<br/><br/>
-- Örnek 1: id'si 1 olan çalışanın adını güncelleme<br/>
UPDATE employee SET name = 'Ahmet Kobroviç' WHERE id = 1;<br/><br/>
-- Örnek 2: id'si 10 olan çalışanın doğum gününü güncelleme<br/>
UPDATE employee SET birthday = '1980-01-01' WHERE id = 10;<br/><br/>
-- Örnek 3: id'si 20 olan çalışanın e-postasını güncelleme<br/>
UPDATE employee SET email = 'yeni.email@ornek.com' WHERE id = 20;<br/><br/>
-- Örnek 4: id'si 30 olan çalışanın adını ve doğum gününü güncelleme<br/>
UPDATE employee SET name = 'Zeynep Sasali', birthday = '1994-05-01' WHERE id = 30;<br/><br/>
-- Örnek 5: id'si 40 olan çalışanın adını, doğum gününü ve e-postasını güncelleme<br/>
UPDATE employee SET name = 'Fahri Bahri', birthday = '2000-01-01', email = 'son.yeni.email@ornek.com' WHERE id = 40;<br/><br/><br/>
4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.<br/><br/>
-- Örnek 1: id'si 1 olan çalışanın kaydını silme<br/>
DELETE FROM employee WHERE id = 1;<br/><br/>
-- Örnek 2: Adı 'Ahmet Kobroviç' olan çalışanın kaydını silme<br/>
DELETE FROM employee WHERE name = 'Ahmet Kobroviç';<br/><br/>
-- Örnek 3: Doğum günü '1980-01-01' olan çalışanın kaydını silme<br/>
DELETE FROM employee WHERE birthday = '1980-01-01';<br/><br/>
-- Örnek 4: E-postası 'yeni.email@ornek.com' olan çalışanın kaydını silme<br/>
DELETE FROM employee WHERE email = 'yeni.email@ornek.com';<br/><br/>
-- Örnek 5: Adı 'Zeynep Sasali' olan çalışanın kaydını silme<br/>
DELETE FROM employee WHERE name ='Zeynep Sasali' ;<br/><br/>
