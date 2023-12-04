graph TD
  A[UtilisateurAnonyme] -->|Connexion()| B[BiblioConnect]
  A -->|ProposerOeuvre()| B
  B -->|FormulaireAjoutOeuvre| B
  A -->|RemplirFormulaire()| B
  A -->|SoumettreFormulaire()| B
  B -->|EnregistrerModération()| C[DB]
  B -->|ExamenBibliothecaires()| D[Bibliothecaire]
  D -->|ExaminerDetails()| B
  B -->|ValiderIntegration()| B
  B -->|NotificationRejet| A
