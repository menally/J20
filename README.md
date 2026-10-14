import java.util.ArrayList;
public class Main {
    public static void main(String[] args) {
        ArrayList<String> biblioteca = new ArrayList<>();
        System.out.println("==METODOD .add() en videojugeos");
        biblioteca.add("The legend of zelda");
        biblioteca.add("Minecraf");
        biblioteca.add("Halo infinite");
        biblioteca.add("Elden ring");
        System.out.println("Biblioteca actual:" + biblioteca);

        System.out.println("METODO .get() ==");
        String juegoDestacado = biblioteca.get(0);
        String juegoMultijugador = biblioteca.get(2);

        System.out.println("Juego en la posicion 0:" + juegoDestacado);
        System.out.println("Juego en la posicion 2" + juegoMultijugador);

        System.out.println("\n=== METODO .set()==");
        biblioteca.set(2, "Terraria");
        System.out.println("Biblioteca tras actualizar la posicion 2:" + biblioteca);

        System.out.println("\n===  METODO .remove () ==");
        biblioteca.remove(0);
        System.out.println("Despues de eliminar el juego de la posicion 0:" + biblioteca);
        biblioteca.remove("Hola infinite");
        System.out.println("Despues de eliminar 'Halo infinite' por nombre:" + biblioteca);

        System.out.println("\n=== ESTADO FINAL DE LA BIBLIOTECA===");
        System.out.println("Total de juegos disponibles (.size()):" + biblioteca.size());
        System.out.println("Lista final de videojuegos:" + biblioteca);
    }
}