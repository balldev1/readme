### TrueFalse =>

<div>
    {Product.length === 0 ? (
        <div>True</div>              <= true
    ) : (
        <div>False</div>             <= false
    )}
</div>

### Map =>

<div>
    {Products.map((product,index)=>(
        <div key={index}>
            {product.item}
        </div>
    ))}
</div>

### Input Search =>

=> get value search

const [searchValue, setSearchValue] = useState<string>('');

=> value product

const filteredProducts = products.filter((product: any) =>
product.name.toLowerCase().startsWith(searchValue.toLowerCase())
);

input value={searchValue} onChange={(e) => setSearchValue(e.target.value)}>

### interface {} =>

interface Product {
name : string;
sprites : { <= Value {} => sprites
front_default: { <= How to call Api => sprites.front_default.test
test : string
}
}
}

### interface {[]} =>

interface Product {
type :{
slot : number;
type : {
name: string;
url : string;
};
}[]; <= Tab Close []
}

### useState interface =>

const [ products, setProducts] = useState<Product[]>([]);

### axios try catch useEffect async =>

const [ products , setProducts ] = useState([]) <= useState

useEffect(()=>{
const fetchData = async() =>
try{
const ProductArray = []
const response = axios.get('http') <= axios

            ProductArray.push(response.Data);               <= response.data
            setProducts(ProductArray);                      <= SetState

        } catch (error){
            console.error("Error",error);
        }
    }

 <!-- } -->

)

### or many Product =>

useEffect(()=>{

    const fecthData = async() =>{

        try{
            const ProductArray = []
            const CountProduct = 16

            for(let i=0;i<=CountProduct;i++){
            const response = axios.get('http')

            ProductArray.push(response.data);
           }
           setProduct(ProductArray)

        }catch
    }

})

### Dynamic Routes Params Id =>

=> Button
button onClick={() => router.push(`/monster/detail/${index}`)}>

=> Structure
detail => [id] => page.tsx

=> Page
const DetailPage = ({params}:Params) =>

const DetailId = params.id <= Params

${parseInt(monsterId) + 1 <= Int Params เพราะรับค่า string มาต้องบวก 1 เพือดึงข้อมูล api / 1
}
