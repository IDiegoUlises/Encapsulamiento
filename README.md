# Encapsulamiento

La encapsulación es un concepto de programación orientada a objetos en los datos de la función y la manipulación de los datos unidas entre sí, así que para evitar la interferencia externa y el mal uso, garantizando así la seguridad. encapsulación de datos salen de otros importantes conceptos de POO, a saber,ocultación de datos.

Protegido (Protected): Podemos decir que estás no son de acceso público, solamente son accesibles dentro de su clase y por subclases.

Privado (Private): En este nivel se puede declarar miembros accesibles sólo para la propia clase.

```c++
class Encapsulado
{
  private:
    int x;

  public:
    void set(int a)
    {
      x = a;
    }

    int get()
    {
      return x;
    }
};
void setup()
{
  Serial.begin(9600);
}

void loop()
{
  Encapsulado objeto;

  objeto.set(5);
  Serial.println(objeto.get());
  delay(1000);
}
```


