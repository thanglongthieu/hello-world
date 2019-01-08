# hello-world
my repository
Hi, everybody!
i'm a newcomer of github. i want to make friend with all but my English is too bad. 
BUT.... i'm willing to fight English to make friend to you.
Thank in advance.....!
function sort_number( arr ){
  return arr.sort(function(a,b){
    return a - b ;
  }) ;
}
function true_number( arr ){
  return arr.every(function(item){ 
        return item > 0 ;
  })
}
describe('arithmetic functions', function(){
  let input, output;
  beforeEach(function () { 
    console.log('beforeEach ran') ;
    input = [ 1, 2, 3, 4, 9, 6, 5, 1, 3, 5 ] ;
    output = [ 1, 1, 2, 3, 3, 4, 5, 5, 6, 9 ] ;
  })
  afterEach(function () { 
    console.log('Test Done !') ;
    input = null ;
    output = null ;
  })
  it('return true number > 0', function(){
     expect(true_number( input )).toBe( true );
  })
  it('return sort', function(){
     expect(sort_number( input )).toEqual( output );
  })  
});
