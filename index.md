<style>
/* === 3-column layout === */
.page-layout {
  display: grid;
  grid-template-columns: 220px 1fr 250px; /* left | center | right */
  gap: 20px;
  margin: 40px;
}

/* Left Sidebar */
.left-sidebar {
  position: fixed;
  top: 30px;
  left: 30px;
  width: 200px;
}

/* Right Sidebar */
.right-sidebar {
  position: fixed;
  top: 30px;
  right: 30px;
  width: 220px;
}

/* Main Content */
.main-content {
  margin: 0 auto;
  max-width: 800px;
}
</style>
