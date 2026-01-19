---
layout: custom
title: What We Believe
---

{% include nav.html %}


# James: 5 Canons
1. **Christ is Lord, not Capital.**  
2. Sin is embedded in economic and political systems. 
3. Christian should resist exploitative wealth and systems that crush workers and the poor.  
4. God hears the harvesters’ cries and will bring about justice.  
5. The Gospel requires preaching repentance, generosity, solidarity, and good news to the poor.  
6. Faithful obedience requires churches, workers, and neighbors to follow Jesus in action toward mercy, equity, and hope.


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
        Christian anti-capitalism is the conviction that Christ is Lord over economic life, and that any system
        that normalizes exploitation, domination, or the treating of workers as disposable contradicts the Gospel.
        It names the spiritual danger of Mammon, rejects profit as the highest good, and insists that economic
        arrangements must serve human dignity and the common good.
      </p>

      <details class="learn-more">
        <summary>Learn more</summary>
        <div class="learn-more-body">
          <h4>Key Scriptures</h4>
          <ul>
            <li><strong>James 5:1-6</strong> - Woes to the rich who exploit labor.</li>
            <li><strong>Matthew 6:24</strong> - You cannot serve God and Mammon.</li>
            <li><strong>Luke 4:18-19</strong> - Good news to the poor, liberty to the oppressed.</li>
            <li><strong>Amos 5:24</strong> - Let justice roll down like waters.</li>
          </ul>

          <h4>Notes</h4>
          <p>
            Add a short paragraph that connects these texts to your thesis and the movement’s commitments.
          </p>
        </div>
      </details>
    </div>

    <div id="christian-socialism" class="toggle-panel">
      <h3>Christian Socialism</h3>
      <p>
        Christian socialism is the practice of organizing political and economic life around solidarity, justice,
        and material care for the vulnerable, grounded in the lordship of Christ. It emphasizes the social
        obligations of wealth, the priority of workers and families, and the call to build institutions that
        distribute power and provision more fairly.
      </p>

      <details class="learn-more">
        <summary>Learn more</summary>
        <div class="learn-more-body">
          <h4>Key Scriptures</h4>
          <ul>
            <li><strong>James 5:1-6</strong> - Woes to the rich who exploit labor.</li>
            <li><strong>Matthew 6:24</strong> - You cannot serve God and Mammon.</li>
            <li><strong>Luke 4:18-19</strong> - Good news to the poor, liberty to the oppressed.</li>
            <li><strong>Amos 5:24</strong> - Let justice roll down like waters.</li>
          </ul>

          <h4>Notes</h4>
          <p>
            Add a short paragraph that connects these texts to your thesis and the movement’s commitments.
          </p>
        </div>
      </details>
    </div>
  </div>
</section>


<script>
(function(){
  const block = document.currentScript.previousElementSibling;
  if (!block || !block.classList.contains('toggle-block')) return;

  const buttons = block.querySelectorAll('.toggle-btn');
  const panelsWrap = block.querySelector('.toggle-panels');
  const panels  = block.querySelectorAll('.toggle-panel');

  function closeAll(){
    panels.forEach(p => p.classList.remove('is-open'));
    buttons.forEach(b => b.classList.remove('is-active'));
    panelsWrap.classList.remove('is-open');
  }

  buttons.forEach(btn => {
    btn.addEventListener('click', () => {
      const targetId = btn.dataset.target;
      const panel = block.querySelector('#' + targetId);
      const wasOpen = panel.classList.contains('is-open');

      closeAll();

      if (!wasOpen){
        panel.classList.add('is-open');
        btn.classList.add('is-active');
        panelsWrap.classList.add('is-open');
      }
    });
  });
})();
</script>

<section class="comparison-block">
  <h3>What do different traditions say about…</h3>

<table class="comparison-table js-expandable-table">
  <thead>
    <tr>
      <th>Question</th>
      <th>Capitalism</th>
      <th>Materialist Socialism</th>
      <th class="highlight-col">Christian Socialism</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td><strong>To whom does your labor belong?</strong></td>

      <td class="expandable" data-detail="labor" data-col="capitalism">
        Your employer
      </td>

      <td class="expandable" data-detail="labor" data-col="materialist">
        The collective
      </td>

      <td class="expandable highlight-col" data-detail="labor" data-col="christian">
        God
      </td>
    </tr>

    <tr class="detail-row" data-detail-row="labor">
      <td colspan="4">
        <div class="detail-box">
          <h4>Expanded explanation - Labor</h4>

          <p class="detail-lede">
            This is the longer explanation that appears under the row you clicked.
            You can write it neutrally, then add your Christian framing.
          </p>

          <div class="detail-grid">
            <div>
              <h5>Capitalism</h5>
              <p>
                Contractually, labor is exchanged for wages and directed by the employer. This can create clarity and
                efficiency, but can also treat the worker primarily as an input to production.
              </p>
            </div>

            <div>
              <h5>Materialist</h5>
              <p>
                Labor is oriented toward collective production and planned ends, with authority typically centered in
                party-state institutions.
              </p>
            </div>

            <div>
              <h5>Christian Socialism</h5>
              <p>
                Labor is ultimately rendered to God and offered for neighbor-love. The worker is not owned - they are a
                steward of vocation. Economic arrangements are judged by whether they honor dignity and serve the common good.
              </p>
              <p class="detail-verses">
                Suggested texts - James 5:1-6, Matthew 6:24, Colossians 3:23-24
              </p>
            </div>
          </div>
        </div>
      </td>
    </tr>

      <tr>
        <td><strong>What is labor for?</strong></td>
        <td>Profit</td>
        <td>Planned production</td>
        <td class="highlight-col">Love of neighbor</td>
      </tr>

      <tr>
        <td><strong>View of the worker</strong></td>
        <td>Economic unit</td>
        <td>Class actor</td>
        <td class="highlight-col">Image-bearer of God</td>
      </tr>

      <tr>
        <td><strong>View of wealth</strong></td>
        <td>Private accumulation</td>
        <td>Collective control</td>
        <td class="highlight-col">A burden of responsibility</td>
      </tr>

      <tr>
        <td><strong>Ultimate authority</strong></td>
        <td>The market</td>
        <td>The party / state</td>
        <td class="highlight-col">Christ</td>
      </tr>
    </tbody>
  </table>
  <p>While Marxism, Leninism, and Maoism differ in important ways, they share a materialist view of labor, history, and authority that distinguishes them from Christian Socialism’s theological foundation.</p>
</section>

<script>
(function(){
  const table = document.querySelector('.js-expandable-table');
  if (!table) return;

  const detailRows = table.querySelectorAll('.detail-row');

  function closeAll(){
    detailRows.forEach(r => r.classList.remove('is-open'));
  }

  table.addEventListener('click', (e) => {
    const cell = e.target.closest('td.expandable');
    if (!cell || !table.contains(cell)) return;

    const id = cell.dataset.detail;
    if (!id) return;

    const row = table.querySelector(`.detail-row[data-detail-row="${id}"]`);
    if (!row) return;

    const wasOpen = row.classList.contains('is-open');

    closeAll();
    if (!wasOpen) row.classList.add('is-open');
  });
})();
</script>
