int empezarmarco = 0;
PImage[] marco = new PImage[12];
int tiempo = 0;

void setup() {
  size(500, 500);
  strokeWeight(4);
  smooth();
  background(204);
  for (int i = 0; i < marco.length; i++) {
    marco[i] = get(); // crea un marco en blanco
  }
}

void draw() {
  int currentTiempo = millis();
  if (currentTiempo > tiempo + 100) {
    siguientemarco();
    tiempo = currentTiempo;
  }
  if (mousePressed == true) {
    line(pmouseX, pmouseY, mouseX, mouseY);
  }
}

void siguientemarco() {
  marco[empezarmarco] = get(); // la ventana
  empezarmarco++; // Incrementa
  if (empezarmarco >= marco.length) {
    empezarmarco = 0;
  }
  image(marco[empezarmarco], 0, 0);
}
