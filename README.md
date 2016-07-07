function onCreateView(rootContainer){
  var view = document.createElement('canvas');
  ...
  return view;
}

function onRender(view, data){
    ...
    myChart.data.datasets[0].data.push(data.total_users);
    myChart.update();
    ...
}