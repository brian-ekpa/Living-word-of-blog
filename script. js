const posts = [
  {
    title: "Today's Message: Faith in Trials",
    content: "Faith is the substance of things hoped for, the evidence of things not seen. When we face trials, our faith is tested. Will we trust God even when things don't go our way?...",
    full: "Faith is the substance of things hoped for, the evidence of things not seen. When we face trials, our faith is tested. Will we trust God even when things don't go our way? Remember, God's plans are for good. Stay firm in Him and let your faith grow stronger in the fire. James 1:2-4 tells us to count it all joy when we face trials because they produce perseverance. Let perseverance finish its work."
  },
  {
    title: "God’s Love Never Fails",
    content: "The love of God is deeper than any ocean and wider than any sky. No matter where you are in life, His love is there for you...",
    full: "The love of God is deeper than any ocean and wider than any sky. No matter where you are in life, His love is there for you. Nothing can separate us from the love of God — not trouble, hardship, or fear. Romans 8:38-39 reminds us that neither death nor life can separate us from His love."
  }
];

let currentIndex = 0;

function renderPost(index) {
  const container = document.getElementById("message-container");
  const post = posts[index];
  container.innerHTML = `
    <h2>${post.title}</h2>
    <p>${post.content} <span class="read-more" onclick="readMore(${index})">Read more</span></p>
  `;
}

function readMore(index) {
  const container = document.getElementById("message-container");
  const post = posts[index];
  container.innerHTML = `
    <h2>${post.title}</h2>
    <p>${post.full}</p>
  `;
}

function nextPost() {
  if (currentIndex < posts.length - 1) {
    currentIndex++;
    renderPost(currentIndex);
  }
}

function prevPost() {
  if (currentIndex > 0) {
    currentIndex--;
    renderPost(currentIndex);
  }
}

window.onload = () => renderPost(currentIndex);
