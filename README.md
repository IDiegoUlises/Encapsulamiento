# Encapsulamiento

La encapsulacion es un concepto de programacion orientada a objetos en los datos y la manipulacion de los datos para evitar la interferencia externa y el mal uso, garantizando asi la seguridad con la ocultacion de datos.

* Publico (Public): Acceso desde cualquier clase.
* Protegido (Protected): Estas no son de acceso publico, solamente son accesibles dentro de su clase y por subclases.
* Privado (Private): En este nivel se puede declarar miembros accesibles solo para la propia clase.

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


