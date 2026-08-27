/* ==========================================
   VARIABLES DE COLOR Y CONFIGURACIÓN BASE
   ================================---------- */
:root {
  --bg-dark: #0a0f1d;
  --bg-card: #131b2e;
  --bg-input: #1a2540;
  
  /* Colores vivos inspirados en reacciones químicas */
  --neon-blue: #00f0ff;   /* Fuego de mechero Bunsen */
  --neon-green: #39ff14;  /* Soluciones fluorescentes / Cobre */
  --neon-pink: #ff007f;  /* Oxidación / Indicadores */
  --neon-purple: #bd00ff; /* Permanganato potásico */
  --neon-yellow: #ffe600; /* Reacciones energéticas */
  
  --text-main: #ffffff;
  --text-muted: #94a3b8;
  
  --border-color: rgba(0, 240, 255, 0.2);
  --glow-shadow: 0 0 15px rgba(0, 240, 255, 0.3);
}

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
}

body {
  background-color: var(--bg-dark);
  color: var(--text-main);
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
}

/* ==========================================
   CONTENEDOR PRINCIPAL Y TARJETAS
   ================================---------- */
.container {
  width: 100%;
  max-width: 900px;
}

.card {
  background-color: var(--bg-card);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 2rem;
  margin-bottom: 1.5rem;
  box-shadow: var(--glow-shadow);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-3px);
  box-shadow: 0 0 25px rgba(0, 240, 255, 0.5);
}

h1, h2, h3 {
  color: var(--neon-blue);
  margin-bottom: 1rem;
  text-shadow: 0 0 10px rgba(0, 240, 255, 0.4);
}

/* ==========================================
   FORMULARIOS Y ENTRADAS (REACTIVOS)
   ================================---------- */
.input-group {
  display: flex;
  gap: 1rem;
  margin-bottom: 1.5rem;
}

input, select {
  flex: 1;
  background-color: var(--bg-input);
  border: 1px solid var(--border-color);
  border-radius: 8px;
  padding: 0.8rem 1rem;
  color: var(--text-main);
  font-size: 1rem;
  outline: none;
  transition: border-color 0.3s, box-shadow 0.3s;
}

input:focus, select:focus {
  border-color: var(--neon-green);
  box-shadow: 0 0 10px rgba(57, 255, 20, 0.4);
}

/* ==========================================
   BOTONES VIBRANTES
   ================================---------- */
.btn {
  background: linear-gradient(135deg, var(--neon-blue), var(--neon-purple));
  color: var(--bg-dark);
  font-weight: bold;
  border: none;
  border-radius: 8px;
  padding: 0.8rem 1.5rem;
  cursor: pointer;
  text-transform: uppercase;
  letter-spacing: 1px;
  transition: all 0.3s ease;
  box-shadow: 0 0 10px rgba(189, 0, 255, 0.4);
}

.btn:hover {
  filter: brightness(1.2);
  box-shadow: 0 0 20px var(--neon-purple);
  transform: scale(1.02);
}

.btn-danger {
  background: linear-gradient(135deg, var(--neon-pink), var(--neon-yellow));
  box-shadow: 0 0 10px rgba(255, 0, 127, 0.4);
}

/* ==========================================
   ÁREA DE RESULTADOS Y ECUACIONES
   ================================---------- */
.reaction-output {
  background: rgba(0, 0, 0, 0.4);
  border-left: 4px solid var(--neon-green);
  padding: 1.5rem;
  border-radius: 0 8px 8px 0;
  font-family: 'Courier New', Courier, monospace;
  font-size: 1.2rem;
  margin-top: 1rem;
  color: var(--neon-green);
  text-shadow: 0 0 8px rgba(57, 255, 20, 0.3);
}

/* Etiquetas de elementos o estados */
.badge {
  display: inline-block;
  padding: 0.3rem 0.6rem;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: bold;
  background-color: var(--bg-input);
  border: 1px solid var(--neon-pink);
  color: var(--neon-pink);
  margin-right: 0.5rem;
}