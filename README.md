1-	Chave PK da tabela tb_customer é a coluna Id_customer, Chave PK da tabela dm_adress_type é a coluna cd_address_type.
2-	INSERT INTO id_customer VALUES (1,’Joaozinho Silva’,88877766655)

INSERT INTO id_customer_andress (id_customer, cd_andress_type, street, lot, zip_code)
VALUES (1, ‘R’, ‘Rua das Flores’, 1, 01234567)

INSERT INTO id_customer_andress VALUES (1,’C’,’Rua das Pedras’,100,’conjunto 200’,01234567)
3-	Podem ser cadastrados 3 tipos de endereços: R – Residencial, C – Comercial e O – Outros.
4-	DELETE FROM tb_customer_adress
WHERE id_customer = (SELECT id_customer FROM tb_customer 
WHERE cpf_cnpj = 888777666555) 

DELETE FROM tb_customer
WHERE cpf_cnpj = 88877766655
