BudgetPrecision

EN

Description:
BudgetPrecision is a Python program compiled into an executable (.exe) that reconstructs point positions from measured distances between them and generates a DXF drawing along with an error analysis report.

Prerequisites:
- Windows 10 or later
- CSV file with columns: p1, p2, d
- Python 3.13+ (if using the script version)
- Python libraries: numpy, ezdxf (if using the Python version)
- Executable: BudgetPrecision.exe
- Optional: DXF viewer (AutoCAD, FreeCAD, LibreCAD...)

Required Files:
- distances.csv: Default distance file.
  Each line must contain:
  p1,p2,d
  O,D,100.0
  A,B,50.0
  …
- You can rename the input CSV or output DXF files, but you must pass the new names as arguments.

Usage via executable:
1. Place BudgetPrecision.exe and the CSV file in the same folder.
2. Double-click BudgetPrecision.exe to run with default names:
   - Input CSV: distances.csv
   - Output DXF: result.dxf
3. To use custom file names:
   BudgetPrecision.exe my_file.csv output.dxf
4. The program automatically generates a text report named _corrections.txt containing:
   - Final coordinates of each point
   - RMS error and relative error compared to initial distances
   - Error propagation analysis via simulation

Generated Results:
- DXF file containing:
  - A circle for each point
  - Point name label
  - Lines connecting points with known distances
- Text file: _corrections.txt detailing all adjustments and analyses

Notes:
- Points O and D are mandatory as fixed references.
- The program automatically adjusts point positions to minimize overall error.
- It can be used for various point sets as long as distances are provided in the CSV.
- To modify the DXF appearance (colors, sizes), adjust the Python script before compilation.

Important Antivirus Note:
If your antivirus flags BudgetPrecision.exe as a threat, don't panic — it’s just being extra cautious. It is NOT a virus, we promise. To allow it on Windows:
1. Open Windows Security → Virus & Threat Protection.
2. Click Protection history, find BudgetPrecision.exe and choose Allow on device.
3. Relax, grab a coffee, your computer is safe.

FR

Description :
BudgetPrecision est un programme Python compilé en exécutable (.exe) permettant de reconstruire les positions de points à partir de distances mesurées entre eux et de générer un dessin DXF ainsi qu’un rapport d’analyse des erreurs.

Pré-requis :
- Windows 10 ou supérieur
- Fichier CSV avec colonnes : p1, p2, d
- Python 3.13+ (si vous utilisez la version script)
- Bibliothèques Python : numpy, ezdxf (si vous utilisez la version Python)
- Exécutable : BudgetPrecision.exe
- Optionnel : Visualiseur DXF (AutoCAD, FreeCAD, LibreCAD…)

Fichiers attendus :
- distances.csv : fichier de distances par défaut.
  Chaque ligne doit contenir :
  p1,p2,d
  O,D,100.0
  A,B,50.0
  …
- Vous pouvez renommer le fichier CSV ou DXF de sortie mais assurez-vous de passer les noms en arguments.

Usage via exécutable :
1. Placer BudgetPrecision.exe et le fichier CSV dans le même dossier.
2. Double-cliquer sur BudgetPrecision.exe pour exécuter avec les noms par défaut :
   - CSV : distances.csv
   - DXF de sortie : result.dxf
3. Pour utiliser des noms personnalisés :
   BudgetPrecision.exe mon_fichier.csv sortie.dxf
4. Le programme génère automatiquement un rapport texte _corrections.txt avec :
   - Coordonnées finales de chaque point
   - Erreur RMS et erreur relative par rapport aux distances initiales
   - Analyse de propagation d’erreur par simulation

Résultats générés :
- DXF avec :
  - Cercle pour chaque point
  - Nom du point
  - Lignes reliant les points dont la distance est connue
- Fichier texte : _corrections.txt détaillant toutes les corrections et analyses

Remarques :
- Les points O et D sont obligatoires comme référence fixe.
- Le programme ajuste automatiquement les positions pour minimiser l’erreur globale.
- Peut être utilisé pour différents jeux de points tant que les distances sont fournies dans le CSV.
- Pour modifier l’apparence du DXF, ajustez les couleurs et tailles dans le script Python avant compilation.

Note importante antivirus :
Si votre antivirus détecte BudgetPrecision.exe comme une menace, ne paniquez pas — il est juste trop prudent. Ce N’EST PAS un virus, promis. Pour l’autoriser sur Windows :
1. Ouvrez Sécurité Windows → Protection contre les virus et menaces.
2. Cliquez sur Historique de protection, trouvez BudgetPrecision.exe et choisissez Autoriser sur l’appareil.
3. Respirez, prenez un café, votre ordinateur est en sécurité.
