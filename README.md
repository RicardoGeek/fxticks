# MYSQL DATABSE

```sql
CREATE DATABASE '[YOUR PREFERRED NAME]';

CREATE TABLE `ticks`.`tick` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `bid` VARCHAR(45) NOT NULL,
  `ask` VARCHAR(45) NOT NULL,
  `pair` VARCHAR(45) NOT NULL,
  `time` DATETIME NOT NULL,
  `ema20` VARCHAR(45) NULL,
  PRIMARY KEY (`id`));

CREATE TABLE `ticks`.`flag` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `userid` VARCHAR(45) NOT NULL,
  `type` VARCHAR(45) NOT NULL,
  `status` VARCHAR(45) NOT NULL,
  PRIMARY KEY (`id`));

CREATE TABLE `ticks`.`user` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `username` VARCHAR(45) NOT NULL,
  `password` VARCHAR(145) NOT NULL,
  PRIMARY KEY (`id`));
```