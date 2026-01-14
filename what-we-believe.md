---
layout: custom
title: What We Believe
---

{% include nav.html %}


# James: 5 Canons
We confess: **Christ is Lord, not Capital.**  
We resist: exploitative wealth and systems that crush workers and the poor.  
We proclaim: God hears the harvesters’ cries.  
We practice: repentance, generosity, solidarity, and good news to the poor.  
We invite: churches, workers, and neighbors to follow Jesus in public—toward mercy, equity, and hope.


<section class="toggle-block">
  <div class="toggle-buttons">
    <button type="button" class="toggle-btn is-active" data-target="anti-cap">
      What is Christian Anti-Capitalism
    </button>
    <button type="button" class="toggle-btn" data-target="christian-socialism">
      What is Christian Socialism
    </button>
  </div>

  <div class="toggle-panels">
    <div id="anti-cap" class="toggle-panel is-open">
      <h3>Christian Anti-Capitalism</h3>
      <p>
        <!-- Replace this with your copy -->
        Christian anti-capitalism is the conviction that Christ is Lord over economic life, and that any system
        that normalizes exploitation, domination, or the treating of workers as disposable contradicts the Gospel.
        It names the spiritual danger of Mammon, rejects profit as the highest good, and insists that economic
        arrangements must serve human dignity and the common good.
      </p>
    </div>

    <div id="christian-socialism" class="toggle-panel">
      <h3>Christian Socialism</h3>
      <p>
        <!-- Replace this with your copy -->
        Christian socialism is the practice of organizing political and economic life around solidarity, justice,
        and material care for the vulnerable, grounded in the lordship of Christ. It emphasizes the social
        obligations of wealth, the priority of workers and families, and the call to build institutions that
        distribute power and provision more fairly.
      </p>
    </div>
  </div>
</section>

<script>
(function(){
  const root = document.currentScript.previousElementSibling;
  if (!root || !root.classList.contains('toggle-block')) return;

  const buttons = root.querySelectorAll('.toggle-btn');
  const panels  = root.querySelectorAll('.toggle-panel');

  function openPanel(id){
    panels.forEach(p => p.classList.toggle('is-open', p.id === id));
    buttons.forEach(b => b.classList.toggle('is-active', b.dataset.target === id));
  }

  buttons.forEach(btn => {
    btn.addEventListener('click', () => openPanel(btn.dataset.target));
  });

  // Ensure only one is open on load
  openPanel(root.querySelector('.toggle-btn.is-active')?.dataset.target || panels[0].id);
})();
</script>
