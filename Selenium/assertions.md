assertions
==========
Cuando una aserción falla, no se lanza una excepción pero se registra el fallo. Llamar a assertAll() hará que se lance una excepción si falla al menos una aserción.
SoftAssert s = new SoftAssert();
s.assertTrue(False, "mensaje");
s.assertAll();
