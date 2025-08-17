/* ===========================
   Glow / Néon pour Voiceflow
   =========================== */

/* Couleur du glow (R G B) — modifie ici si besoin */
:root {
  --vf-glow: 0 200 255;   /* cyan */
  --vf-bg:   10 14 24;    /* fond sombre pour un meilleur rendu */
}

/* --- Bouton flottant (launcher) --- */
.vfrc-launcher {
  background: rgb(var(--vf-bg)) !important;
  border: 1.5px solid rgba(var(--vf-glow), 0.8) !important;
  box-shadow:
    0 0 0 1px rgba(var(--vf-glow), 0.9),
    0 0 16px rgba(var(--vf-glow), 0.8),
    0 0 36px rgba(var(--vf-glow), 0.5) !important;
  transition: transform .2s ease, box-shadow .2s ease;
}
.vfrc-launcher:hover {
  transform: translateY(-1px);
  box-shadow:
    0 0 0 2px rgba(var(--vf-glow), 1),
    0 0 24px rgba(var(--vf-glow), 1),
    0 0 60px rgba(var(--vf-glow), 0.6) !important;
}
/* petit glow sur l’icône */
.vfrc-launcher svg { filter: drop-shadow(0 0 6px rgba(var(--vf-glow), 0.9)); }

/* --- Fenêtre du chat (contour + ombre lumineuse) --- */
/* On cible plusieurs conteneurs possibles du widget pour couvrir les variantes */
#voiceflow-chat .vfrc-chat,
#voiceflow-chat .vfrc-widget,
#voiceflow-chat .vfrc-chat--dialog,
#voiceflow-chat .vfrc-modal,
#voiceflow-chat .vfrc-frame {
  border-radius: 18px !important;
  border: 1.5px solid rgba(var(--vf-glow), 0.75) !important;
  box-shadow:
    0 0 0 1px rgba(var(--vf-glow), 0.8),
    0 0 28px rgba(var(--vf-glow), 0.55),
    0 0 60px rgba(var(--vf-glow), 0.35),
    0 0 90px rgba(var(--vf-glow), 0.25) !important;
  overflow: hidden;
  background:
    radial-gradient(120% 100% at 10% 0%, rgba(var(--vf-glow), .10) 0, transparent 60%),
    rgb(var(--vf-bg)) !important; /* fond très léger pour faire ressortir l’effet */
}

/* Header et zone d’input : léger glow intérieur pour la cohérence */
#voiceflow-chat .vfrc-header,
#voiceflow-chat .vfrc-footer,
#voiceflow-chat .vfrc-composer {
  background: rgba(15, 23, 42, 0.72) !important;
  backdrop-filter: blur(6px);
  border-top: 1px solid rgba(var(--vf-glow), .25);
  border-bottom: 1px solid rgba(var(--vf-glow), .25);
  box-shadow: inset 0 0 12px rgba(var(--vf-glow), .15);
}

/* (Optionnel) Animation de “respiration” douce au survol de la fenêtre */
@keyframes vf-pulse {
  0%, 100% {
    box-shadow:
      0 0 0 1px rgba(var(--vf-glow), 0.8),
      0 0 28px rgba(var(--vf-glow), 0.55),
      0 0 60px rgba(var(--vf-glow), 0.35);
  }
  50% {
    box-shadow:
      0 0 0 2px rgba(var(--vf-glow), 1),
      0 0 40px rgba(var(--vf-glow), 0.8),
      0 0 90px rgba(var(--vf-glow), 0.5);
  }
}
#voiceflow-chat .vfrc-chat:hover,
#voiceflow-chat .vfrc-widget:hover,
#voiceflow-chat .vfrc-chat--dialog:hover {
  animation: vf-pulse 3s ease-in-out infinite;
}

/* (Optionnel) Déclinaisons de couleurs rapides */
:root.theme-violet  { --vf-glow: 155 100 255; }
:root.theme-rose    { --vf-glow: 255 70 170;  }
:root.theme-vert    { --vf-glow: 0 255 170;   }
