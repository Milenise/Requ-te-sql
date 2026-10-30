CREATE TABLE utilisateurs (
    nom VARCHAR(100) NOT NULL,
    prenom VARCHAR(100) NOT NULL,
    age INT(11) NOT NULL,
    date_naissance DATE NOT NULL,
    adresse VARCHAR(250) NOT NULL,
    email VARCHAR(100) NOT NULL
);

CREATE TABLE tvs (
    nom_tv VARCHAR(150) NOT NULL,
    marque_tv VARCHAR(50) NOT NULL,
    taille FLOAT(20) NOT NULL
);

CREATE TABLE smartphones (
    nom_smartphone VARCHAR(150) NOT NULL,
    marque_smartphone VARCHAR(50) NOT NULL,
    couleur VARCHAR(20) NOT NULL
);



ALTER TABLE smartphones
CHANGE couleur date_de_sortie DATE NOT NULL;



ALTER TABLE utilisateurs
ADD id_utilisateurs INT NOT NULL AUTO_INCREMENT PRIMARY KEY FIRST;

ALTER TABLE tvs
ADD id_tvs INT NOT NULL AUTO_INCREMENT PRIMARY KEY FIRST;

ALTER TABLE smartphones
ADD id_smartphones INT NOT NULL AUTO_INCREMENT PRIMARY KEY FIRST;




INSERT INTO utilisateur
(id_nomde_laTable, Nom, Prénom, Age, date_of_birth, adresse, email)
VALUES
(1, 'Greg', 'Gui', 25, '2001-03-15', '12 Rue de Paris, Bruxelles', 'greg.gui@gmail.com'),
(2, 'MoHamed', 'sala', 30, '1996-07-22', '45 Avenue Louise, Bruxelles', 'Mohamed.sala@gmail.com'),
(3, 'Marco', 'spano', 25, '2001-02-01', '8 Rue Royale, Bruxelles', 'Marco.spano@gmail.com');





INSERT INTO tvs
(id_nomdelatable, Nom_de_tv, Marque_tv, taille)
VALUES
(1, 'S90D', 'Samsung', 65),
(2, 'OLED55C4', 'LG', 55),
(3, 'Bravia 9 XR90', 'Sony', 75);





INSERT INTO smartphone
(id_nomdelatable, Nom_smartphone, marque_smartphone, date_de_sortie)
VALUES
(1, 'iPhone 16', 'Apple', '2024-09-20'),
(2, 'Galaxy S25', 'Samsung', '2025-02-01'),
(3, 'Pixel 9', 'Google', '2024-08-22');