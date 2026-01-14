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
    <button type="button" class="toggle-btn" data-target="anti-cap">
      What is Christian Anti-Capitalism
    </button>
    <button type="button" class="toggle-btn" data-target="christian-socialism">
      What is Christian Socialism
    </button>
  </div>

  <div class="toggle-panels">
    <div id="anti-cap" class="toggle-panel">
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
  const block = document.currentScript.previousElementSibling;
  if (!block || !block.classList.contains('toggle-block')) return;

  const buttons = block.querySelectorAll('.toggle-btn');
  const panels  = block.querySelectorAll('.toggle-panel');

  function closeAll(){
    panels.forEach(p => p.classList.remove('is-open'));
    buttons.forEach(b => b.classList.remove('is-active'));
  }

  buttons.forEach(btn => {
    btn.addEventListener('click', () => {
      const targetId = btn.dataset.target;
      const panel = block.querySelector('#' + targetId);
      const isOpen = panel.classList.contains('is-open');

      closeAll();

      // If it was not open, open it. If it was open, leave all closed.
      if (!isOpen){
        panel.classList.add('is-open');
        btn.classList.add('is-active');
      }
    });
  });
})();
</script>

