<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <title>Befundgenerator HWS</title>
  <style>
    body { font-family: sans-serif; margin: 40px; }
    label, select, button, textarea { display: block; margin-top: 15px; width: 100%; }
    textarea { height: 150px; }
  </style>
</head>
<body>

  <h2>🧠 HWS-Befundgenerator</h2>
  <p>Bitte wähle die klinischen Befundmerkmale aus:</p>

  <label>Druckschmerz:</label>
  <select id="druck">
    <option value="">nicht eintragen</option>
    <option value="Paravertebraler Druckschmerz im mittleren HWS-Bereich.">vorhanden</option>
    <option value="Kein Druckschmerz der HWS.">nicht vorhanden</option>
  </select>

  <label>Beweglichkeit:</label>
  <select id="beweglichkeit">
    <option value="">nicht eintragen</option>
    <option value="Beweglichkeit der HWS schmerzbedingt eingeschränkt.">eingeschränkt</option>
    <option value="Beweglichkeit der HWS frei.">frei</option>
  </select>

  <label>Neurologischer Befund:</label>
  <select id="neurologie">
    <option value="">nicht eintragen</option>
    <option value="pDMS beidseits erhalten, kein neurologisches Defizit.">unauffällig</option>
    <option value="Sensibilitätsstörung im Bereich C6 links.">auffällig</option>
  </select>

  <button onclick="generiereBefund()">📝 Befund generieren</button>

  <textarea id="ausgabe" placeholder="Hier erscheint dein Befundtext..."></textarea>

  <script>
    function generiereBefund() {
      let druck = document.getElementById('druck').value;
      let beweg = document.getElementById('beweglichkeit').value;
      let neuro = document.getElementById('neurologie').value;
      let text = [druck, beweg, neuro].filter(Boolean).join(' ');
      document.getElementById('ausgabe').value = text;
    }
  </script>

</body>
</html>
